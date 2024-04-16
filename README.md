# ScreenShort-with-TimerSetup
When you execute this script, you will be prompted to input the delay time. After setting the delay period, it will wait for that time before taking a screenshot. When the delay time is up, it takes a screenshot, shows it, and saves it as "myscreenshorts.png" in the current directory.

import pyscreenshot: This imports the  pyscreenshort library, which captures screenshots.

import time: This imports the time module, which is required for time-related methods.
 
Delay = int(input("Enter the delay time for screen short:")): This line allows the user to specify the delay time (in seconds) before taking the snapshot. The input() method accepts user input, and int() converts it to an integer.
print(f"Waiting for {delay} seconds before taking screenshot..."): This line displays the amount of seconds the script will wait before taking a screenshot. It formats the message using f-strings based on the delay variable.
time.Sleep(delay): This line pauses the script's execution for the supplied delay period.It waits for the user-specified period before capturing the screenshot.

image = pyscreenshot.grab(): This code uses the pyscreenshot library's grab() method to take a snapshot of the full screen. The taken screenshot is saved in the image variable.

image.show(): This line displays the taken screenshot using your system's default image viewer.

image.save("myscreenshorts.png"): This line saves the screenshot as "myscreenshorts.png" to the current directory. The save() method is used to store the screenshot under the supplied filename. 


