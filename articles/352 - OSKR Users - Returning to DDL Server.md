# OSKR Users - Returning to DDL Server

# Returning to DDL Server (OSKR Users)

These steps will provide you a pathway to return to the standard DDL server and leave the Escape Pod in the event that you need to. These steps are specialized to minimize collateral damage to other development work in your currently loaded firmware; you can [CLICK HERE for steps](https://oskr.ddl.io/oom/doc/unlock_checklist.html#deploy-3-deploying-the-latest-oskr-software-ota-image) on reflashing the firmware to the latest OSKR build if you have not made any changes to your OSKR firmware.
 *Note: You will still need to run a Clear User Data reset on Vector to reconnect to the DDL server.*

Basic Requirements:
 -SSH Access to Vector ( **Note: Vector*****must*****be on OSKR firmware to continue.**)
 -Original server\_config.json file (stored on the Vector robot in the */anki/data/assets/cozmo\_resources/config/*directory)

1. SSH into your Vector and mount as read-write:
    *$ mount -o remount rw /*
2. Revert server\_config.json to its original endpoints:
    *$ cd /anki/data/assets/cozmo\_resources/config/
    $ cp server\_config.json.orig server\_config.json*
3. Clear User Data:
   1. Place Vector on his Charger.
   2. Double tap his Back button.
   3. Gently lift his arm assembly all the way up, then lower it back down.
   4. Rotate one of his treads until “Clear User Data” is highlighted.
   5. Gently lift his arm assembly all the way up, then lower it back down.
   6. Confirm the wipe by rotating Vector's tread again to select "Confirm".
   7. Gently lift his arm assembly all the way up, then lower it back down.
4. Connect to Vector using [Vector-Web-Setup](//support.digitaldreamlabs.com/article/114-video-vector-and-connection-how-to-set-vector-up) (You must use Google Chrome for this.)
   1. **Note**: A Bluetooth-enabled PC is required for this. If you do not have a Bluetooth-enabled PC, please use the [Vector Robot mobile app](//support.digitaldreamlabs.com/article/114-video-vector-and-connection-how-to-set-vector-up).
   2. Place Vector on his Charger.
   3. Double tap his Back button.
   4. Click "Pair With Vector", then input the 4-digit pairing PIN that appears on Vector's screen into Vector-Web-Setup.
   5. Finish onboarding by moving through the prompts and selecting your preferences. If you are asked to log in, use the credentials that you use on the Vector Robot mobile app.
