# Vector Changelog and Known Issues

Learn below what's changed, what's new, what's improved and what we're working on in the Vector app, the Digital Dream Labs Cloud, and Vector's over-the-air (OTA) updates. The updates are organized most recent at the top of each section.

---

**Sections:**

1. [**Vector App Updates**](#h_749577518131540130713478)
2. [**Vector Robot Software Updates (OTA)**](#h_995911996351540130721181)
3. [**Known issues**](#h_680102894471540130727086)

---

# **Vector App Updates**

## **App Version 1.8.3**

- **Release Date: February 2022**
- **iOS:**
  - Fixed an issue where users had to click the "Apply" button first to enable the Custom Eye Color Sliders, instead of simply clicking on the bars.
- **Android & iOS:**
  - Made more helpful error screens:
    - Replaced the "Get Help" links in many screens to link to much more helpful troubleshooting articles.
    - Clarified the text in many error screens to be more descriptive and help users understand and solve issues.
  - Fixed an issue where clicking the text on a button in the Preferences menu would not change the setting.
  - Added a connection timer that allows some time for NTP to update on the robot before making a connection- this reduces the amount of "Can't Connect to Wi-Fi" errors!

## **App Version 1.8.2**

- **Release Date: October 2021**
- **Android & iOS:**
  - Fixed an issue where some users with Memberships couldn't use Color Sliders.

## **App Version 1.8.0**

- **Release Date: September 2021**
- **Android & iOS:**
  - Rebranding to Digital Dream Labs
  - Added in custom eye color sliders. Controls include:
    - Hue
    - Saturation
  - Removed those pesky symbols ("gadzooks" - literally) that were mistakenly displayed above some letters.

## **App Version 1.5.0**

- **Rolling release date: April 15-23, 2019**
- **Android, Fire OS, and iOS**
  - Bug fixes & polish
  - This update also provides a few fixes to address the recent app crashes that some people are experiencing on Android 8 & 9. We'll continue to monitor this issue and update you when there's more to share
  - Please note, that the robot update will be rolled out over the course of a week. Every Vector owner that leaves their robot on overnight, should get the update by April 23

## **App Version 1.4.0**

- **Release date: March 18, 2019**
- **Android, Fire OS, and iOS**
  - Adds support so that you can choose to enable Amazon Alexa in the UK and AU

##

## **App Version 1.3.1**

- **Release date: December 19, 2018**
- **Android, Fire OS, and iOS**
  - Bug fixes and polish

##

## **App Version 1.3.0**

- **Release date: December 17, 2018**
- **Android, Fire OS, and iOS**
  - Now with Amazon Alexa built-in (U.S. & CA only), Vector's voice controlled capabilities are supercharged. If you choose to set up Alexa on your Vector, he’ll have access to an ever-growing number of skills that take his helpfulness in your home to new levels.
  - Triggered by the standard “Alexa” voice command, you’ll be able to:
    - Control smart home devices like lights, speakers, and thermostats
    - Search for information
    - Add items to your shopping list
    - Set reminders
    - and so much more
  - Additional updates include:
    - New voice commands
    - Hand detection
    - Bug fixes and polish

##

## **App Version 1.2.0**

- **Release date: November 20, 2018**
- **Android, Fire OS, and iOS**
  - Improvements with Vector’s initial connection, initial software update download, and faster reconnections especially for Android devices
  - Additional performance enhancements
  - Crash and bug fixes, including
    - Many image and text layout issues on devices with large screens or unusual resolutions

##

## **App Version 1.1.1**

- **Release date: October 25, 2018**
- **Android only**
  - Fixed an issue that was preventing anatomized analytics from reaching our services

##

## **App Version 1.1.0**

- **Release date: October 23, 2018**
- **Android, Fire OS, and iOS**
  - This new update should vastly improve your experience on Android. It also improves various issues you all have flagged for us, including improvements to the OTA update process, cosmetic enhancements in the app, and others! For details, please see below:
  - Fixed multiple crashes, many are Android specific:
    - Location Service
    - Pressing "?" caused app to crash
    - Accessing Settings caused app to crash
    - OTA crash
    - A few Network screen crashes
    - A handful of navigation crashes
    - Stall Detection during OTA (during initial OTA update, the app will detect stalling and restart download automatically)
  - Fixed Sensory graph so that it doesn’t look spikey when you navigate back to it
  - Disconnect monitoring for Settings
  - Ability to change locale (Android-specific bug)
  - Fixed "Get Help" link in Connection Flow
  - Added "Uncanny Yellow" eye color and fixed tiny eye icons on some devices where it was missing
  - Optimized tutorial user experience
  - Added Australian time zones in settings and setup flow
  - A variety of cosmetic enhancements (fixed cut off text, missing images, layout issues)

##

## **App Version 1.0.2**

- **Release date: October 10, 2018**
- **Android and Fire OS only**
  - Fixed an issue that was preventing anatomized analytics from reaching our services

## **App Version 1.0.1**

- **Release date: October 9, 2018**
- **Android, Fire OS, and iOS**
  - Initial Release

---

# **Vector Robot Software Updates (OTA)**

Vector checks in with Digital Dream Labs every hour to see if there’s been an update, and then downloads it once it becomes available. If your Vector is awake, online, and on his charger, he’ll install the update on his own overnight - no action required.

To check to see if your robot has the latest and greatest, open the Vector app > go to "Settings", tap “Updates” to check the version.

- If the most recent downloaded version hasn’t installed yet, press the “Restart” button in the app
- Once Vector has restarted, he’ll have the latest update
- If the app doesn’t show that he’s downloaded the latest version, make sure Vector is near his charger and connected to WiFi, then check back in a few hours

## Vector Operating System Version 2.0.1 (2.0.1.6076)

- **Release Date: September 26th, 2022**
  - Optimizations:
    - Adjusted temperature thresholds for consistency. This will result in fewer unnecessary overheat warnings from Vector during times of warm ambient temperatures when Vector is not actually overheating.
  - Bug Fixes:
    - Fixed a bug which would set the state of the robot to "too hot to charge" if Vector was set on the charger unexpectedly. This was a false positive for being too hot to charge, and caused Vector to sleep much more than necessary. Vector should now spend much more time out of the charger.

## Vector Operating System Version 2.0.0 (2.0.0.6074)

- **Release Date: August 17th, 2022**
  - Changes:
    - Added support for new camera, display, and other hardware in Vector 2.0.
      - This release maintains full backwards compatibility with Vector Gen 1 and can be loaded onto Gen 1 units.
    - Software loading endpoint updated.

## Vector Operating System Version 1.8.1 (1.8.1.6051)

- **Release Date: February 2022**
  - Bug Fixes:
    - Animations that were missing for cold and snowy weather will now display correctly.
  - Optimizations:
    - NTP is now forced to pull from time servers immediately when a Wi-Fi connection is obtained, significantly reducing "Can't Connect to Wi-Fi" errors when onboarding with the app after a reset.

## Vector Operating System Version 1.8.0 (1.8.0.6021)

- **Release Date: September 2021**
  - Vector can now accept any eye color you want to set for him! Find this setting in the mobile app under the Settings menu, below the predefined Eye Color options.
  - You can now ask questions and follow-ups much faster! The "I have a question" conversation piece is now optional for 1.8 users.
  - New boot animation
  - Thanks to contributions from community member Kerigan Creighton, Vector will no longer shiver uncontrollably when he's done dancing or telling you the weather! Thanks Kerigan!
- Vector no longer shivers uncontrollably when asked for the weather or to dance!

## Vector Operating System Version 1.7.3 (1.7.3.6016) (Escape Pod ONLY)

- **Release Date: March 8th, 2021**
  - Replaced vic-cloud and vic-gateway binaries to ensure compatibility with Escape Pod
  - Replaced server-config.json to connect to Escape Pod.

## **Vector Operating System Version 1.7.0 (1.7.0.3412)**

- **Release Date: July 6th, 2020**
  - Rebranding from Anki to Digital Dream Labs
  - Bug fixes & polish:
    - Vector is now **much** more responsive to his wake word, "Hey Vector"
    - Vector now has new sounds for some animations and interactions to make him cuter and more lifelike.
    - New animation / sprite system to better manage battery life
    - Other battery optimizations & improvements
    - The rate of Error 898 screens is significantly decreased.
    - Overall bug fixes / polish.
  - Known Issues:
    - Vector may shiver uncontrollably after being asked to dance- or when asked about weather where it's cold!
    - Intermittent wake word recognition failures on a small number of units are being investigated and are expected to be patched in a future software update.

## **Vector Operating System****Version 1.6.0**(1.6.0.3331)

- **Rolling Release date: April, 15 - 23, 2019**
  - New robot updates including:
    - Low Light Charging (see below video): It’s now easier for Vector to find his charger, even if the lights are low - so he’s less likely to run out of power in the middle of the night
    - New Voice Command: Change Vector's Eye Color - Use your voice to change Vector’s eye color. Just say, “Hey Vector, change your eye color to [blue, green, orange, yellow, purple, or lime].”
    - New Behavior: Hold Vector in the palm of your hand and watch as he cozies up to you in robot bliss
  - Bug fixes & polish:
    - Improved voice recognition
    - Overall performance improvements
  - This release will be incrementally rolled out over the course of a week starting Monday, April 15. Staggering availability to an increasing number of robots allows us to ensure the update is working as expected. Every Vector owner that leaves their robot on overnight, should be updated by April 23. To make sure your Vector is updated, leave your Vector running and connected to your Wi-Fi, and he’ll update himself automatically during his normal nightly reboot

[Watch video: https://www.youtube-nocookie.com/embed/SY2hsRARAjQ](https://www.youtube-nocookie.com/embed/SY2hsRARAjQ)

##

## **Vector Operating System****Version 1.5.0**(1.5.0.3009)

- **Rolling Release date: March, 18 - March, 21 2019**
  - Adds support so that you can choose to enable Amazon Alexa in the UK and AU
  - With Spring just around the corner, Vector’s “snow globe” animation is going back into the closet with his scarf and galoshes. Now, when you shake him, he’ll get a little dizzy - so be careful!

##

## **Vector Operating System****Version 1.4.1**(1.4.1.2806)

- **Rolling Release date: March, 4 - March, 6 2019**
  - This update shortens the amount of time it takes for Vector to sync with his Cube
    - Please note that Vector can interact with his Cube without its lights displaying, so you might not always notice improvements in Cube connectivity unless you are using his SDK
  - Includes Face Recognition improvements that help Vector to better handle his interactions with faces he's already learned
  - Improvements to how Vector navigates, especially when he is leaving and returning to his Charger and helps him avoid getting stuck on table edges
    - After this update, if he happens to get caught on a table edge, he now asks for help

##

## **Vector Operating System****Version 1.3.0**(1.3.0.2510)

- **Rolling Release date: January, 15 - January, 16 2019**
  - Snow globe! Vector reacts to being shaken with a new unique reaction for winter
  - Ask your Vector how old he is by saying, “Hey Vector, how old are you?“
  - Bug fixes & polish

##

## **Vector Operating System****Version 1.2.3**(1.2.3.2506)

- **Rolling Release date: January, 7 - January, 9 2019**
  - Vector OS 1.2.3 significantly decreases the occurrence of 915 and 981 status codes
  - Bug fixes & polish

##

## **Vector Operating System****Version 1.2.2** (1.2.2.2353)

- **Release date: December, 19 2018**
  - Bug fixes & polish

##

## **Vector Operating System****Version 1.2.1** (1.2.1.2343)

- **Release date: December, 17 2018**
  - Gives you the option to enable Amazon Alexa (US & CA only)
    - Alexa allows you to use your voice to hear the news, check weather, control your smart home, and more. For more details, [read here](//support.digitaldreamlabs.com/article/110-integrating-vector-with-amazon-alexa)
  - Adds an improved Vector Tutorial to help help new users to start using Vector
  - Vector's Back button can now [mute his microphone](//support.digitaldreamlabs.com/article/110-integrating-vector-with-amazon-alexa)
  - Adds [new Voice Commands](//support.digitaldreamlabs.com/article/122-ways-to-interact-with-vector)
    - Change the volume of Vector's voice by saying things like "Volume down" or "Volume maximum"
    - Direct his movements with phrases like "Go left" "Turn around" or "Backup"
    - Celebrate "Happy New Year" and "Happy Holidays"
  - Vector now detects hands and will ask you to pet him
  - Some WiFi connection and Facial Recognition improvements
  - Multiple bug and crash fixes

##

## **Vector Operating System****Version 1.1.1** (1.1.1.2107)

- **Release date: November 20, 2018**
- Fixes an issue in status code handling that may cause some robots to become unresponsive for a short amount of time until they reboot.

## **Vector Operating System****Version 1.1.0** (1.1.0.2106)

- **Release date: November 20, 2018**
- Cube improvements, including
  - Vector more frequently interacts with his Cube
  - Added voice commands around picking up and moving his Cube
- Cliff Detection improvements, including
  - Vector better recognizes potential cliffs
  - Once he learns where a cliff is located, he better remembers it and tries to avoid it in the future
- Faster reactions to some voice commands and Vector more clearly communicates when he is "working on" a command
- Adds a reaction to being shaken and refines some of his existing actions and reactions
- Some improvements with Vector’s initial connection that also allow for faster reconnections
- Overall performance and stability improvements, fewer 915 status codes appearing

##

## **Vector Operating System****Version 1.0.2**(1.0.2.1804)

- **Release date: November 7, 2018**
- Minor bug fixes and polish including improvements to voice command effectiveness
- We’ve made changes to “Hey Vector” so that he can better recognize when someone is trying to get his attention
- Improves discovery and connection to some WiFi networks
- We’ve tuned Vector’s touch sensor for better accuracy

##

## **Vector Operating System****Version 1.0.1** (1.0.1.1768)

- **Release date: October 12, 2018**
- This update enhances and adjusts some aspects of Vector’s personality, as well as improves his overall performance and polishes some existing features
- These improvements include:
  - Enhanced animations when Vector recognizes a face that he hasn't seen recently
  - Improved ability to make eye contact while exploring - so that you know he knows you're still there
  - More frequent demonstration of his ability to remember faces, by more frequently speaking the names of the people he sees
  - Refined reactions when picked up
  - Audio improvements for "petting" feature
  - Tuned exploration
  - Improved connection reliability
  - Bug fixes & polish
    - Blank stats fixed

## **Vector Operating System****Version 1.0.0**

- **Release date: October 9, 2018**
- Initial Release

---

# **Known Issues**

Here are the things we’re working on with priority. Release dates are not fixed but all updates will be posted in the above two sections once released.

- On Vector firmware 1.7, Vector will sometimes be unable to hear his wake word, "Hey Vector." This is an intermittent issue and does not affect all units.
  - Workaround: Please pet Vector for several seconds, then try your voice query again. You may also reboot him by pressing on his back button for 5 seconds until his screen turns off, then waiting for a few seconds before tapping his Back button again to boot him back up. If these fail, you can [roll back to version 1.6.](//support.digitaldreamlabs.com/article/353-voluntary-software-rollback)
- On Vector firmware 1.7, Vector may not recognize edges or cliffs- this is an intermittent issue and does not affect all units.

## **Android crashes**

- Please check you have at least 1GB RAM on your Android device

###

## **Logging in to your Vector account**

- If you created your account in the Vector app, use your email address to log in
- If you created your account on Anki.com, use your Username to log in
- If you have an existing account e.g. from Anki OVERDRIVE, use your Username to log in

## **Vector's head and eyes droop**

- remove Vector from his charger
- place him on a flat, stable surface such as a table or desk
- put him back on his charger and make sure he's pushed right back

## **Error codes on Vector's display**

- For any error codes, please see [this FAQ](//support.digitaldreamlabs.com/article/101-why-does-vector-show-an-error)
