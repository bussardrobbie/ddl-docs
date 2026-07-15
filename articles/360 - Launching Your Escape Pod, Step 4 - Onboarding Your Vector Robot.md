# Launching Your Escape Pod, Step 4: Onboarding Your Vector Robot

## Onboarding Your Vector Robot

It's time to connect Vector to the Escape Pod, then update his firmware for Escape Pod!

[Watch video: https://player.vimeo.com/video/512632548](https://player.vimeo.com/video/512632548)

1. Open a web browser window and navigate to [http://escapepod.local](http://escapepod.local/)
   1. **NOTE:**Some Windows computers may not be able to find the Escape Pod's address. If you are on a Windows PC and you cannot visit [http://escapepod.local](http://escapepod.local:):
      1. Please open the Start Menu, then find the "Run" option. You may also press Win+R to bring up the "Run" dialog box.
      2. Insert the following into the dialog box: *reg add "HKLM\Software\Policies\Microsoft\Windows NT\DNSClient" /v EnableMulticast /t REG\_DWORD /d 1 /f*
      3. Click "OK". Reboot your computer and then continue.
2. The Licensing screen will appear.
   1. Click "Add A License To Start"
   2. Copy the License Key obtained from Digital Dream Labs via email and paste it into the text field.
   3. Click "Save".
      1. Note: If you need to add multiple licenses, use the "Add License" button at the top of the page before continuing. You can add more licenses at any time.
3. Boot Vector into Firmware Recovery (**skip this if upgrading from Escape Pod 1.0**):
   1. Place Vector onto his charger.
   2. Press and hold Vector’s Back Button for around 15 seconds in total until the rectangle furthest away from the circle LED lights up blueish white
   3. He will reboot and show "anki.com/v" on his screen
4. Click "Menu", then click "Onboarding."
   1. Place Vector on his charger, then tap his back button twice to enter Pairing Mode.
   2. Click "Pair with Vector"
   3. Use the PIN number that appears on Vector's screen and type it into the PIN Number field, then click "Enter PIN".
      1. Note: If the PIN does not appear within 5 seconds, refresh the page and go back to Step 4.
   4. If Vector is not yet connected to Wi-Fi, you will be prompted to connect to Wi-Fi now:
      1. Click on the Wi-Fi network you want to connect Vector to (network must be on the 2.4GHz frequency)
      2. Type in the password to the network. Passwords are case-sensitive.
      3. Click "Connect Vector to Wi-Fi"
   5. In the Firmware Selection screen, use the drop-down menu to select the firmware file that your robot needs:
      1. Production (Normal) Vectors:
         1. Select the firmware beginning with the word "PROD" and your preferred version number.
      2. OSKR (unlocked) Vectors:
         1. Select the firmware beginning with the word "OSKR" and your preferred version number.
         2. **NOTE:** OSKR users **MUST** complete additional onboarding steps - follow Step 3 in this article: [OSKR - Onboarding Vector to Escape Pod](//support.digitaldreamlabs.com/article/349-escape-pod-robot-onboarding-oskr)
   6. Click the "Upload Firmware to Vector" button.
      1. Vector will begin loading the new firmware.
         1. Note: This process may take between 5 and 20 minutes, depending on your network speed. When firmware loading is complete, you will return to the "Pair with Vector" screen.
   7. Clear Vector's User Data (**you may not have to do this if you are upgrading to Escape Pod 1.8.2**):
      1. Place Vector on his charger and plug the charger in
      2. [If Vector is booting up, wait for the “V” to finish]
      3. Double click Vector’s Back Button
      4. Gently raise and lower Vector’s lift
      5. Turn his treads to move through selections (backwards to go up, forwards to go down)
      6. Raise and lower the lift to select the “Clear User Data” menu
      7. Confirm the selection and wait for Vector to reboot
      8. Once Vector completes rebooting, data will have been wiped from the robot
   8. Connect Vector via Bluetooth again:
      1. Place Vector on his charger, then tap his back button twice to enter Pairing Mode.
      2. Click "Pair with Vector"
      3. Use the PIN number that appears on Vector's screen and type it into the PIN Number field, then click "Enter PIN".
         1. Note: If the PIN does not appear within 5 seconds, refresh the page and go back to Step 4h.
   9. You will be prompted to connect to Wi-Fi now:
      1. Click on the Wi-Fi network you want to connect Vector to (network must be on the 2.4GHz frequency)
      2. Type in the password to the network. Passwords are case-sensitive.
      3. Click "Connect Vector to Wi-Fi"
   10. In the Firmware Selection screen, click "Skip To Next Step"
   11. Click "Activate Your Robot", which will appear within a few seconds.
   12. Select the Preferences that you will use for Vector:
       1. Locale Options:
          1. en-US (United States)
          2. en-GB (Great Britain / UK)
          3. en-AU (Australia)
       2. Select from available Time Zones
       3. Select your preferred Temperature Units:
          1. Fahrenheit
          2. Celsius
       4. Select your preferred Distance Units:
          1. Imperial
          2. Metric
       5. Enter your Default Location
          1. Note: Default Location is used for weather or other functions when the Escape Pod Extension Engine is running.
       6. Select the Back Button Behavior
       7. Select the remainder of your preferences, then click "Save Settings"

### You're all done! All voice commands will now be routed to the Escape Pod.
