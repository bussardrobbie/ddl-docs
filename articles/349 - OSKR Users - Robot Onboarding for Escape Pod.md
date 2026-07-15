# OSKR Users - Robot Onboarding for Escape Pod

# Vector Robot Configuration

Here we will learn how to use OSKR to point Vector to the Escape Pod.

 ***Before continuing, please be familiar with the current Known Issues and Limitations. See***[Known Issues and Limitations](//support.digitaldreamlabs.com/article/351-known-issues)

 **Basic Requirements:**
 -SSH Access to Vector (Note: Vector ***must***be on OSKR firmware to continue.)
 -Escape Pod Invitation Email

1. License your Vector:
   1. Check your email for an Escape Pod license invitation. Use the linked form to submit your email address and serial number to Digital Dream Labs- please be sure to use the email address that your purchase was made with.
      1. Note: If using Gmail, be sure to check your Updates and Promotions tabs!
   2. You will receive an email with a text file that contains your license string.
   3. If you have not already done so, [CLICK HERE to complete the setup for your Raspberry Pi](//support.digitaldreamlabs.com/article/350-oskr-users-pi-flashing-for-the-escape-pod)- this will need to be done to continue in the process. You can continue through Steps 2 and 3 while waiting for your license string.
   4. Open a new tab in your browser and connect to <http://escapepod.local>
   5. Click “Add A License To Start”
   6. Submit license code into the text box on the “Licenses” Screen, and click "Save".
2. Install the required binaries
    (**Complete this inside the Vector Robot)**
    **NOTE: Step 2 is NOT required if you are on OSKR firmware 1.8 or above with the Pod- skip to Step 3.**
   1. Download the [vic-cloud and vic-gateway binaries](https://github.com/digital-dream-labs/vector-cloud/releases/tag/v1.0.0)
   2. SSH into your Vector and mount as read-write:
       *$ mount -o remount rw /*
   3. CREATE BACKUPS of existing vic-cloud and vic-gateway files in /anki/bin:
       *$ mv /anki/bin/vic-cloud /anki/bin/vic-cloud.orig* *$ mv /anki/bin/vic-gateway /anki/bin/vic-gateway.orig*
   4. From a command line window on your local computer, use scp to transfer the downloaded vic-cloud and vic-gateway files from your computer to Vector. We are going to transfer these from your PC into the /anki/bin directory on the robot. **Be sure to start this process inside the local computer directory where the vic-cloud and vic-gateway files are stored, or provide an absolute path to vic-cloud and vic-gateway files**:
       *$ scp -i <SSH key path> vic-cloud root@<IP>:/anki/bin
       *$ scp -i <SSH key path> vic-gateway root@<IP>:/anki/bin**
      1. Note: Be sure to change "<SSH key path>" to the path where your Vector's SSH key is stored. Change "<IP>" to the internal IP address of your Vector robot.
   5. Switch back to the command line window inside Vector. Using SSH, set permissions and ownership of the files we just transferred to him:
       *$ cd /anki/bin* *$ chown cloud:anki /anki/bin/vic-cloud* *$ chown net:anki /anki/bin/vic-gateway* *$ chmod 755 /anki/bin/vic-gateway* *$ chmod 755 /anki/bin/vic-cloud*
3. Replace existing server\_config.json contents:
    (**Complete this inside the Vector Robot)**
   1. If you haven't already done so, SSH into your Vector and mount as read-write:
       *$ mount -o remount rw /*
   2. Change directory to find the file: *$ cd /anki/data/assets/cozmo\_resources/config/*
   3. Change permissions of the server\_config.json file to enable editing: *$ chmod u+w /anki/data/assets/cozmo\_resources/config/server\_config.json*
   4. ***CREATE BACKUP*** of existing server\_config.json: *$ cp /anki/data/assets/cozmo\_resources/config/server\_config.json /anki/data/assets/cozmo\_resources/config/server\_config.json.orig*
   5. Edit server\_config.json to point to Escape Pod: *$ nano /anki/data/assets/cozmo\_resources/config/server\_config.json* The contents should be as follows:
       `{ "jdocs": "escapepod.local:443", "tms": "escapepod.local:443", "chipper": "escapepod.local:443", "check": "escapepod.local:80/ok", "logfiles": "s3://anki-device-logs-prod/victor", "appkey": "oDoa0quieSeir6goowai7f" }`
   6. Use "Ctrl+X" to escape Nano and use "y" to save changes. When asked what name you want to give the file, press Enter to leave it as is.
4. Perform Clear User Data:
   1. Place Vector on his Charger.
   2. Double tap his Back button.
   3. Gently lift his arm assembly all the way up, then lower it back down.
   4. Rotate one of his treads until “Clear User Data” is highlighted.
   5. Gently lift his arm assembly all the way up, then lower it back down.
   6. Confirm the wipe by rotating Vector's tread again to select "Confirm".
   7. Gently lift his arm assembly all the way up, then lower it back down.

       *Vector will reboot and the ddl.io/v onboarding screen will appear.*
5. Roll through Vector-Web-Setup to finalize onboarding
   1. Connect to <http://escapepod.local> and click on “Onboarding” in the top right corner.
   2. With Vector on his Charger, double tap his back button.
   3. Click "Pair with Vector", then select the correct Vector name from the dialog box that appears.
   4. Set the desired settings, then click "Activate Your Robot!"
   5. Select your robot variables.
   6. Have fun! Submit feedback, including bugs, ideas, and suggestions to: escapepodbeta@digitaldreamlabs.com
