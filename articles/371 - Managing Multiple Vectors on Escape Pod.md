# Managing Multiple Vectors on Escape Pod

The Escape Pod is designed to be able to manage multiple Vectors, but by default is configured to run 1 Vector at a time. Each Vector requires a process as a listener if you want more than one Vector to hear and answer simultaneously. If there are not enough listening processes set, then the next audio clip will be interpreted as soon as a listener becomes free of its previous task.

 Think of these listeners as lanes in a highway, with the audio clips from 2 Vector robots acting as cars: If you have two cars occupying the same lane, one must follow the other toward the destination, and one cannot pass the other, but they will both arrive at the destination, one after the other. This would be if you have 1 listener running. If you have 2 listeners running, then you have just added a lane to your highway, and both cars can travel at the same speed without getting in the way of one another. Thus, we're assuming that for each Vector in the same room, you'd run 1 listener, because we expect that each Vector in the room would hear you when you say his wake word, "Hey Vector." You'd run 2 listeners for 2 Vectors in the same room, etc.

Since each listener will require additional resources on the Pi to run, for performance reasons we recommend following the below table:

| Amount of Vector Robots | Recommended Amount of Pi RAM |
| --- | --- |
| 2 | 2GB |
| 5 | 4GB |
| 6+ (limit 19) | 8GB |

To set the amount of Vectors that you need to run simultaneously, please perform the following steps. These steps are for Windows 10 but will be similar on all platforms:

 **Note**: Mac & Linux users, you can skip to Step 2. You have SSH installed already!

1. Install SSH tools:
   1. Open the Start Menu from the Start Button (usually in the lower left hand corner of your desktop screen)
   2. Search for "Optional" and select "Manage Optional Features" when it appears.
   3. Type "OpenSSH" into the search bar and check the box next to "OpenSSH Client"
   4. Click "Install". OpenSSH will be installed. You may now close the Windows 10 Settings window.
2. Open a Command Prompt or Terminal session from the Start Menu:
   1. Open the Start Menu from the Start Button
   2. Search for "Command" and then click on "Command Prompt" once it appears.
      1. **Note**: In Mac & Linux computers, search for "Terminal"
3. Open an SSH connection to the Escape Pod:
   1. Type in "ssh ubuntu@escapepod.local". A connection to the Escape Pod will be opened.
   2. Type your Raspberry Pi password.
      1. **If you have never logged in before**, this will be "ubuntu" by default. Once you log in it will force you to create a new password. Select a password and type it in twice. The window will close and you will need to start back at Step 2 in this article to open a new Command Prompt / Terminal window.
4. Edit the Escape Pod configuration file:
   1. Type "nano /etc/escape-pod.conf" and hit Enter. You will enter a new screen where you can input text. Use the arrow keys to move around the file and use the Enter button to insert new lines where needed.
   2. Using a new line with no other text on it, enter the following, and replace "<number of Vectors>" with the actual amount of processes you need to be able to run:
       "DDL\_SAYWHATNOW\_STT\_POOL\_SIZE=<number of Vectors>" (See Example Below)
   3. Press **Ctrl+X** to Exit the editor.
   4. Press **Y** to save the changes you've made. If you've made a mistake and need to go back into the Editor, press **Ctrl+C**.
   5. Press Enter to confirm and save the file.
5. Reboot the Escape Pod:
   1. Type "sudo reboot" and Press **Enter**. The connection will close. You may now close the Command window.

Wait 2 minutes to ensure a full reboot has taken place, and then the Pod should start the amount of listening processes you have asked for.
