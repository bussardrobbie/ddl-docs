# Onboarding: "Authorization Failed" Error

The "Authorization Failed" Error is generally related to 3-4 root causes, and is usually easy to fix! Let's take a look at the most common causes of the "Authorization Failed" error.

![Authorization Failed](//d33v4339jhl8k0.cloudfront.net/docs/assets/5e3f0b1e2c7d3a7e9ae777f5/images/61e4dd7d79a38f5473fd463a/file-TZfGNVj6Mz.jpg)

---

### Causes:

- Software:
  - An Escape-Pod compatible version of the Vector software has not been installed onto the Robot.
- License:
  - A License (you should have received this in a text file via email) was not applied in the "Licenses" screen.
  - The License that was applied in the License screen does not match the serial number.
- Vector Robot:
  - A Clear User Data reset was not completed during the Onboarding process.
  - **OSKR Units Only:** The server\_config.json file was not changed to point to the address of the Escape Pod.

---

### Resolutions:

1. Check the Software version running on the robot:
   1. Place Vector on his Charger (make sure the Charger is plugged into the wall).
   2. Double tap Vector's Back button to enter Pairing Mode. A key will appear on his screen.
   3. Gently lift his arm and set it back down. A screen with diagnostic information will appear.
   4. After the text "OS" you should see "ep" on the end of the Software version. Example: "1.7.3.6016ep"
   5. If you do **NOT** see "ep" on the end of the Software, please retry loading the Software titled "PROD\_(*version number*)" using the [Onboarding process](//support.digitaldreamlabs.com/article/360-launching-your-escape-pod-4).
      1. **If you are on an OSKR robot, this may not apply to you, as the server configuration file can be modified to accept the Escape Pod without loading new software. Please see the "OSKR Robots Only" section below.**
   6. If you see "ep" on the end of the Software Version, then Escape Pod compatible software is already loaded. Lift Vector's arm and set it down again to exit the diagnostic screen. Move to Step 2.
2. Check the License:
   1. With your web browser pointing to the Escape Pod, click "Menu" at the top right of the Escape Pod interface.
   2. Click "Licenses" in the menu.
   3. Verify that you have a License installed; you should see "vic:" followed by your robot's serial number in the screen, as shown, under the "Licensed Robots" section:![](//d33v4339jhl8k0.cloudfront.net/docs/assets/5e3f0b1e2c7d3a7e9ae777f5/images/61e4fac5b54d116b7c397d92/file-B2XvWiK6E0.png)
   4. If you do not have a License installed, please download your License from the "Escape Pod License" email that was sent to you:
      1. Click the "Add License" button on the "Licenses" screen of the Escape Pod.
      2. Open the text file that was sent to you (it should be titled with your robot's serial number).
      3. Copy the **entire contents**of thetext file.
      4. Paste the text file into the "License Key"
   5. Verify that the serial number **exactly** matches the bottom of your robot (see this article with [how to find your serial number](//support.digitaldreamlabs.com/article/338-how-do-i-find-vectors-serial-number)). If your License does not match this format, or does not match your robot's serial number, please Contact Us at support@digitaldreamlabs.com for a new license (or you may reply to the email that your license was attached to). **Please include a photo of the bottom of your robot for the fastest assistance.**
3. If the License looks good, it is possible that the robot was not reset prior to the Onboarding process. Perform a Clear User Data reset:
   1. Follow the steps in [this article](//support.digitaldreamlabs.com/article/384-performing-a-clear-user-data-reset).
   2. Retry the [Escape Pod Onboarding process](//support.digitaldreamlabs.com/article/360-launching-your-escape-pod-4).

---

### Resolutions (OSKR Robots *Only*):

Please ensure that you have covered the steps above in the Standard Robots section before moving into this section. **Be aware that if your Vector has not been unlocked with a custom OSKR image and flashed with new firmware, then this sectionwill not apply to you.**

1. Modify the server\_config.json file on the Vector robot:
   1. Point the Vector robot to the Escape Pod by changing the destination of his voice command requests. Follow **Step 3 only**in [this article](//support.digitaldreamlabs.com/article/349-escape-pod-robot-onboarding-oskr).
   2. Reboot the robot after the server\_config.json has been modified:
      1. Press Vector's Back button for 5 seconds until his screen shuts off completely.
      2. Wait for 10 seconds.
      3. Tap Vector's Back button once to begin the bootup process, which will take approximately 1 minute.
      4. Retry the [Escape Pod Onboarding Process](//support.digitaldreamlabs.com/article/360-launching-your-escape-pod-4). **If you update Vector or reload the current software to the robot you will need to re-complete the process of modifying the server\_config.json file each time.**
      5. If you still have trouble, please Contact Us: support@digitaldreamlabs.com.
