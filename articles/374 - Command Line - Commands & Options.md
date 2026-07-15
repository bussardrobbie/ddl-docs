# Command Line: Commands & Options

The Escape Pod has a simulated Command Line Interface with various onboarding and connection tools that the Escape Pod uses to communicate with Vector. Developers may find these tools handy to troubleshoot issues, complete specific onboarding steps, load firmware, and more. Below is a list of commands available on the Escape Pod.

 To access the Command Line Interface, please see [Switching Views on the Escape Pod](//support.digitaldreamlabs.com/article/372-switching-views-on-escape-pod).

To see available commands in the Command Line Interface when connected to Escape Pod, just type "help" to see these listings!

####

#### Command List Table

| Command | Description | Example |
| --- | --- | --- |
| **ble-connect** | Connect to a Vector that is waiting in pairing mode (used with the 4-character Vector Name). **Requires the argument of Vector's name.** | *ble-connect M4D6* |
| **ble-clear** | Clears stored Bluetooth data. Use this command if ble-connect fails repeatedly. No argument is required. | *ble-clear* |
| **echo** | Displays text to the command line output. Can be used with environment variables that have been set with the **export** command (prefix variables with "$"). | *echo $LAST* |
| **export** | Saves environment variables. Useful for saving and mapping text or number values like directories and other commonly needed values. | *export ZERO=0* |
| **printenv** | Lists all environment variables that have been saved before with the **export** command. No argument is required. | *printenv* |
| **unset** | Removes or clears an environment variable. It will no longer be usable, and will no longer be listed when typing **printenv.** You will need to use **export** to define the variable again to use it. | *unset ZERO* |
| **wifi-scan** | Commands Vector to scan for nearby Wi-Fi access points / networks that he can connect to. No argument is required. | *wifi-scan* |
| **wifi-connect** | Commands Vector to connect to a nearby Wi-Fi access point / network discovered using the **wifi-scan** command. Follow the command with the SSID and passphrase of the network, separated by a space (see example to the right). | *wifi-connect network\_name network\_password* |
| **ota-start** | Starts an Over-The-Air (OTA) update to Vector to install new firmware and then will trigger a reboot. The firmware installed will depend on the firmware link or name that is specified after the command. The example to the right installs the latest OSKR firmware onto Vector, then reboots him. | *ota-start http://ota.global.anki-services.com/vic/oskr/full/latest.ota* |
| **ota-cancel** | Cancels the process of an Over-The-Air update (OTA) while it is running. Vector will stay booted into his current firmware. No argument is required. | *ota-cancel* |
| **logs** | Downloads a log package from Vector. These logs are useful in troubleshooting and may be requested by the Customer Care team at Digital Dream Labs. No argument is required. | *logs* |
| **status** | Displays Vector's current status, including the firmware that he is currently running and the network that he is connected to (denoted by the "ssid:" field). No argument is required. | *status* |
