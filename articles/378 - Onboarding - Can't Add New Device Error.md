# Onboarding: "Can't Add New Device" Error

![](//d33v4339jhl8k0.cloudfront.net/docs/assets/5e3f0b1e2c7d3a7e9ae777f5/images/606cc941e0324b5fdfd082b7/file-YELENcZVr6.png)

During Escape Pod Onboarding, you may occasionally see an error that says "can't add new device: can't init hci: no devices available: (hci0: can't up device: connection timed out)". This error means that you may have tried a new pairing connection before the Escape Pod was ready.

#### Solutions:

1. Retry the pairing connection (**Note:** You may need to do this 2-3 times in very rare cases)
   1. Wait for 10 seconds.
   2. Refresh the Onboarding page.
   3. Click "Pair With Vector" again.
2. Reboot the Raspberry Pi:
   1. Locate the power cord for the Raspberry Pi.
   2. Disconnect the power cord from the Raspberry Pi
   3. Wait for 30 seconds.
   4. Re-insert the power cord into the Raspberry Pi.
   5. Wait for 2 minutes for the Pi to finish booting the Escape Pod software.
   6. Refresh the page, then retry pairing with Vector.
