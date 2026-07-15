# Onboarding: "No Devices Found" Error

![](//d33v4339jhl8k0.cloudfront.net/docs/assets/5e3f0b1e2c7d3a7e9ae777f5/images/606cadc78996210f18bd0918/file-UaovvaMnsO.png)

During the Onboarding process, you may see the above error: "No devices were found. Please follow the steps below and try again." This error is generally caused by one of the following issues:

- Vector is not powered on or is not fully booted up.
- Vector is not near enough to the Raspberry Pi (The Escape Pod hardware) to connect via Bluetooth.
- Vector did not send out a Bluetooth signal while the Pi was scanning via Bluetooth.

#### Solutions:

1. Make sure Vector is powered on:
   1. Check for the green light on his back to indicate that he is powered on. If he is on the charger, you may also see three additional green lights rotating. This is normal.
   2. If you have recently powered Vector on (within the last minute or so), give Vector about 1 minute to fully boot, then try again.
2. Move Vector closer to the Escape Pod so that he is within Bluetooth range:
   1. Vector should be within about 15-20 feet of (and preferably in the same room as) the Escape Pod.
   2. You may need to set Vector up on the Escape Pod using a mobile device so that you can be closer to the Escape Pod if your computer is located in another room- or temporarily place Vector on a surface nearer to the Escape Pod for onboarding.
3. Make sure Vector is in pairing mode:
   1. Place Vector on his charger.
   2. Double-tap his back button. He will enter pairing mode and his screen will display a key.
   3. Wait 5 seconds, then click "Pair With Vector" again.
4. If all above steps fail, reboot the Raspberry Pi:
   1. Locate the power cord for the Raspberry Pi.
   2. Disconnect the power cord from the Raspberry Pi
   3. Wait for 30 seconds.
   4. Re-insert the power cord into the Raspberry Pi.
   5. Wait for 2 minutes for the Pi to finish booting the Escape Pod software.
   6. Refresh the page, then retry pairing with Vector.
