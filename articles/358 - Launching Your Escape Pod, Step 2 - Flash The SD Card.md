# Launching Your Escape Pod, Step 2: Flash The SD Card

## Flash the SD Card

Let's prepare the SD card that acts as the hard drive, or data storage space, for your Raspberry Pi. We will flash the Escape Pod image, which contains the operating system and necessary files, to the SD card.

### Download the latest Escape Pod image!

Be sure to [grab the latest Escape Pod image](https://assets.digitaldreamlabs.com/PEavApG5dgnZA5ei/Escape-Pod-Release-1.8.2/ubuntu-20.04.4-escape-pod-1.8.2.img).
 ( ***The current revision at the link above is 1.8.2.***)

[Watch video: https://player.vimeo.com/video/512632352](https://player.vimeo.com/video/512632352)

**Detailed Steps:**

1. Insert the SD card into your SD card reader, then insert the SD card reader into your computer's USB port.
2. Download the latest Escape Pod image from above.
3. Download, install, and run your favorite SD card flashing tool ([BalenaEtcher is recommended](https://www.balena.io/etcher/) for ease of use)
   1. If using BalenaEtcher: Click "Flash From File" on the left hand side of the BalenaEtcher window.
   2. Navigate to the folder where you stored the Escape Pod image (by default, on most computers, this will be your "Downloads" folder).
   3. Click on the Escape Pod image that you downloaded to select it, then click "Open" at the bottom right of the dialog box.
   4. In the BalenaEtcher window, click "Select Target".
   5. Click in the check box on the left hand side to select your SD card.
      1. Tip: Look for "USB Mass Storage Device" or similar name, with a size that is close to your SD card's known size (if you are using a 32GB card, you may see something like "31.9GB")
      2. WARNING: Selecting the incorrect drive or target in this screen can cause damage or loss of data. If you have any questions regarding which target drive to select, do not continue. Contact Digital Dream Labs by emailing us at support@digitaldreamlabs.com for assistance.
4. Configure Wi-Fi (Skip this step if using an Ethernet/LAN cable) before disconnecting the MicroSD card from your computer:
   1. Open a File Explorer and double-click the "system-boot" drive.
      1. If you cannot locate the "system-boot" drive, please disconnect the SD card and reader from your computer and reconnect it.
   2. Find the “network-config” file. Open the file with a standard text editor.
   3. For a fairly standard home Wi-Fi network, uncomment and edit this section. Where "<Your Network Name>" and "<Your Passphrase here>" appear, insert your Wi-Fi network name (SSID) and password between the quotation marks on each line:

      wifis:

         wlan0:

           dhcp4: true

           optional: true

           access-points:

             "<Your Network Name>":

               password: "<Your Passphrase Here>"
   4. Save the file menu by clicking "File" at the top left, then clicking "Save".
   5. Close the text editor, then disconnect the SD card reader from your computer and move to [Section 3: Connecting Your Escape Pod](//support.digitaldreamlabs.com/article/359-launching-your-escape-pod-3).
