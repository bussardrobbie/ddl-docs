# OSKR Users - Pi Flashing for the Escape Pod

# Pi Configuration

With these steps, we will set up the Pi as an Escape Pod. We will flash an image to the Escape Pod, configure Wi-Fi, and boot the Pod.

***Before continuing, please be familiar with the current Known Issues and Limitations. See*** [Known Issues and Limitations](//support.digitaldreamlabs.com/article/351-known-issues)

Basic Requirements:
 -The [latest Escape Pod image](https://assets.digitaldreamlabs.com/PEavApG5dgnZA5ei/Escape-Pod-Release-1.0.0/escape-pod-6ab70e5-R1.img.xz)
 -Pi 4 is *strongly* recommended for performance reasons. Pi 3B / 3B+ can be used as a minimum.
 -Approved Pi power source (5V/2.5A for Pi 3B / 5V/3A for Pi 4)
 -Wi-Fi network, 2.4GHz (Pi 3B / Pi 4) or 5GHz (Pi 4 only)
       OR
 CAT5 (minimum) LAN Ethernet Cable and 1 free LAN port on router ( *Recommended*)
 -MicroSD Card, 8GB or large

*Note: The Pi you use for Escape Pod is designed to run "headless"; that is, with no monitor or other accessories attached- you can simply connect the Pi to your router and access it from any other computer on the same network by opening an internet browser and navigating to*<http://escapepod.local>

1. Flash the image: Download your favorite SD card flashing tool ([BalenaEtcher is recommended](https://www.balena.io/etcher/) for ease of use) and flash the [latest Escape Pod image](https://assets.digitaldreamlabs.com/PEavApG5dgnZA5ei/Escape-Pod-Release-1.0.0/escape-pod-6ab70e5-R1.img.xz) to your MicroSD card.
2. Configure Wi-Fi (Skip this step if using Ethernet/LAN) *before* disconnecting the MicroSD card from your computer:
   1. Mount the "system-boot" partition on the SD card and find the “network-config” file. For a fairly standard home Wi-Fi network, uncomment and edit this section. Where "<Your SSID here>" and "<Your Passphrase here>" appear, insert your Wi-Fi network name (SSID) and password. Please note that the SSID only requires quotation marks around it if you have a space or other special character in the name:

       wifis:

      wlan0

       dchp4: true

       optional: true

       access-points:

       <Your Network Name>:

       password: "<Your Passphrase Here>"
3. Plug in power (and Ethernet, if you skipped Step 2) and boot the Pi. Now you can move on to [Configuring an OSKR Vector for the Escape Pod!](//support.digitaldreamlabs.com/article/349-escape-pod-robot-onboarding-oskr)

---

### SSH Access

If you need to access the Pi via SSH, please use the credentials below.

**Default Credentials:**
 Username: ubuntu
 Password: ubuntu
 *Note: You will be prompted to change these defaults on first login. The connection will automatically exit when you have completed the password change. SSH back into the Pi with your new credentials.*

---

#### *Tailing Escape Pod Logs:*

To tail Escape Pod service logs to diagnose and report issues, use the following shell command:
 `journalctl -u escape_pod.service -f`

To see only the logs that pertain to words that are understood by the Escape Pod (useful in understanding what speech is interpreted to be, and which intent it engages and will be included in a Web UI in a later release), use the following command:
 `journalctl -u escape_pod.service -f | grep incoming_text`
