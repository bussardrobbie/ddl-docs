# Vector Error & Status Codes

Vector will occasionally display an error code (also known as a Status Code) on his screen. These Status Codes are usually nothing to worry about unless they happen often. For troubleshooting, please see this article: [Why Does Vector Show An Error?](//support.digitaldreamlabs.com/article/101-why-does-vector-show-an-error)

*This article was made possible by a combination of internal documentation but also by the work of Randall Maas and his*[Vector Technical Reference Manual](https://github.com/GooeyChickenman/victor/blob/master/documentation/Vector-TRM.pdf)*. Digital Dream Labs wishes to thank Randall for his dedication to the Vector Technical Reference Manual, which is a fantastic resource.*

- 800 - 999
  - If any of these Status Codes consistently appear, there could possibly be a hardware issue with Vector. Startup into Recovery Mode, Clear User Data, and use the Vector app to Reinstall Vector’s OS.
- 700 - 705
  - These are issues triggered by the reading of an internal sensor. A good example would be Vector operating in a room that was too hot.
- 200 - 219
  - If any of these Status Codes appear, they involve Software Updates or the Recovery process. Typically, retrying the Update will fix the issue unless there is a fundamentally more complex issue involved.
- 1 - 10
  - These codes belong to a core Vector service that runs all of Vector’s other services. Most of these codes will never appear on Vector’s display.

---

### Error Code Table

|  |  |  |
| --- | --- | --- |
| **Error Code** | Code Description | **Explanation** |
| **1** | Switchboard: unknown status | Should never happen. |
| **2** | Switchboard: OTA in progress | An Over-The-Air update is currently in progress. |
| **3** | Switchboard: OTA completed | An Over-The-Air Update has completed successfully. |
| **4** | Switchboard: rebooting | The robot is rebooting. |
| **5** | Switchboard: Other OTA error | An unknown error occurred with an Over-The-Update. |
| **10** | OS: Unknown system error |  |
| **200** | Unexpected .tar contents | - Tar file was corrupt - Tar contents did not follow the expected order. |
| **201** | Unhandled manifest version or feature | - Unhandled section format for expansion - The manifest version is not supported - The OTA has the wrong number of images for the type - The OTA is missing a BOOT or SYSTEM image - The manifest configuration is not understood |
| **202** | Boot Control HAL failure | - Could not mark target slot - a or b partition unbootable - Could not set target slot as active |
| **203** | Could not open URL | The URL for the link was invalid (check the link and make sure you can download the OTA on your local machine from the same link) |
| **204** | URL not a TAR file | The URL used to initiate an update pointed to an incorrect filetype. Check the link. |
| **205** | Decompressor error | The .tar/.ota file could not be unpacked- could happen if the .ota file is corrupted. Reboot the robot and try again. |
| **206** | Block error |  |
| **207** | Imgdiff error | Delta payload error |
| **208** | I/O error | - Couldn't sync OS images to disk - Disk error while transferring OTA file |
| **209** | Signature validation error | - Manifest failed signature validation - The aboot, boot image, system image, or delta.bin hash doesn't match the signed manifest (files may have been modified) |
| **210** | Decryption error | Encryption scheme is not supported. |
| **211** | Wrong base version | Vector's current version doesn't match what is expected for this delta update |
| **212** | Subprocess exception | The decompression engine had an unexpected, undefined error. |
| **213** | Wrong serial number | The processor serial number (QSN) is not correct for the robot that the image is being applied to. |
| **214** | Dev / Prod mismatch | Development Vectors can’t install production OTA software, and production Vectors can’t install development OTA software (make sure that you are applying the correct image to Vector). |
| **215** | Socket Timeout (network stall) | OTA transfer failed, due to timeout. (There may be poor network connectivity) |
| **216** | Downgrade not allowed | - The robot is not allowed to upgrade or downgrade from the current version to the new version - OS version name in the update file doesn’t follow an acceptable pattern (the version suffixes – for production, release candidate, userdev, and development – must match the already installed software) |
| **217** |  |  |
| **218** |  |  |
| **219** | Other Exception | Other unexpected, undefined error while transferring OTA file. |
|  |  |  |
| // | Hardware Issues |  |
| **990** | DISPLAY\_FAILURE | The screen could not be detected / initialized (The LCD display is not communicating properly with the processor.) |
| **981** | CAMERA\_STOPPED | - The camera stopped responding to instructions. - mm-anki-camera process hung when the camera stream was exited via vic-engine stop. |
| **980** | CAMERA\_FAILURE | - The camera could not be detected / initialized. - The camera stopped responding to instructions. - mm-anki-camera process hung when the camera stream was exited via vic-engine stop. |
| **970** | WIFI\_HW\_FAILURE | The Wi-Fi radio antenna could not be detected / initialized. |
| **960** | IMU\_FAILUR | The IMU ( [Inertial Measurement Unit](https://en.wikipedia.org/wiki/Inertial_measurement_unit)) could not be detected / initialized. |
|  |  |  |
| // | Vector OS Process Issues |  |
| **923** | NO\_CLOUD\_PROCESS | Vic-cloud failed to start or stopped unexpectedly. |
| **921** | NO\_GATEWAY | Vic-gateway was unable to start or crashed |
| **920** | VIC\_GATEWAY\_CERT | Vic-gateway-cert was unable to generate a x509 certificate for vic-gateway |
| **919** | SYSTEMD | Systemd is not working properly |
| **917** | NO\_ROBOT\_COMMS | - Vic-anim crashed or failed to start. - Vic-robot stopped responding. |
| **916** | NO\_ROBOT\_PROCESS | - Vic-robot was unable to start or crashed |
| **915** | NO\_ENGINE\_COMMS | Vic-engine stopped responding |
| **914** | NO\_ENGINE\_PROCESS | Vic-engine stopped unexpectedly. |
| **913** | NO\_SWITCHBOARD | Vic-switchboard stopped unexpectedly. |
| **911** | AUDIO\_FAILURE | The audio engine stopped unexpectedly or failed to start on boot. |
| **909** | STOP\_BOOT\_ANIM\_FAILED | The boot animation process failed or was unable to start. |
|  |  |  |
| // | Hardware Issues |  |
| **899** | NO\_BODY | - The main board is unable to communicate with the body-board (The cable between boards may be disconnected) - May appear due to a software bug in version 1.6 |
| **898** | SPINE\_SELECT\_TIMEOUT | - The main board is unable to communicate with the body-board (the cable between boards may be disconnected). - This also appears as a software bug in version 1.6. |
|  |  |  |
| // | External Sensor Issues |  |
| **895** | TOUCH\_SENSOR | The back touch sensor failed during power-on self test or during runtime. |
| **894** | TOF | TOF (Time-Of-Flight) sensor failed to initialize or stopped working. |
| **893** | CLIFF\_BL | The back left cliff sensor failed to initialize or stopped working. |
| **892** | CLIFF\_BR | The back right cliff sensor failed to initialize or stopped working. |
| **891** | CLIFF\_FL | The front left cliff sensor failed to initialize or stopped working. |
| **890** | CLIFF\_FR | The front right cliff sensor failed to initialize or stopped working. |
|  |  |  |
| // | Microphone Issues |  |
| **873** | MIC\_BL | Back left microphone failed to initialize / send data. |
| **872** | MIC\_BR | Back right microphone failed to initialize / send data. |
| **871** | MIC\_FL | Front left microphone failed to initialize / send data. |
| **870** | MIC\_FR | Front right microphone failed to initialize / send data. |
|  |  |  |
| // | Cloud Errors |  |
| **852** | CLOUD\_READ\_ESN | There is a problem reading the cloud electronic serial number. |
| **851** | CLOUD\_TOKEN\_STORE | There is a problem with the cloud token store. |
| **850** | CLOUD\_CERT | There is a problem with the cloud certificate. |
|  |  |  |
| // | Manufacturing Issues |  |
| **840** | NO\_CAMERA\_CALIB | The camera is not calibrated. |
|  |  |  |
| // | Vector OS Process Issues |  |
| **801** | DFU\_FAILED | The process to update the cube firmware failed. |
| **800** | NO\_ANIM\_PROCESS | Vic-anim was unable to start or crashed. |
|  |  |  |
| // | Internal Sensor Derived Issues |  |
| **705** | SHUTDOWN\_BATTERY\_CRITICAL\_TEMP | The robot shut down because the battery was too hot to operate safely. |
| **702** | SHUTDOWN\_BATTERY\_CRITICAL\_VOLT | The robot was shut down because the battery voltage was too low. |
| **701** | SHUTDOWN\_GYRO\_NOT\_CALIBRATING | The gyroscope sensor values were out of normal range or the gyroscope failed (it wasn’t able to calibrate), so the robot shut down. |
| **700** | SHUTDOWN\_BUTTON | Normal shutdown due to the button being pressed. |
