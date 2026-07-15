# Firmware Loading: "Downgrade Not Allowed" Error

![](//d33v4339jhl8k0.cloudfront.net/docs/assets/5e3f0b1e2c7d3a7e9ae777f5/images/606cc2624466ce6ddc5f1d55/file-XjjzJz53Ij.png)

The "Downgrade Not Allowed" error may appear when attempting to load firmware from the Escape Pod. This error usually results from the following issue:

- Vector is not booted into the 0.9.0 firmware when attempting to load new firmware files

#### Solution:

1. Boot Vector into Firmware Recovery Mode:
   1. Place Vector onto his charger.
   2. Press and hold Vector’s Back Button for around 15 seconds in total until the rectangle furthest away from the circle LED lights up blueish white
   3. He will reboot and show "anki.com/v" on his screen
2. Enter pairing mode by double-tapping Vector's back button while he is on his charger.
3. Refresh the Onboarding page, then click "Pair With Vector" and try firmware loading again after entering the PIN from Vector's screen.
