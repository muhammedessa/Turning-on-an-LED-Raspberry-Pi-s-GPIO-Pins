# Turning-on-an-LED-Raspberry-Pi-s-GPIO-Pins

Create a new text file “LED.py” by typing the following:

nano LED.py
Type in the following code:

import RPi.GPIO as GPIO
import time
GPIO.setmode(GPIO.BCM)
GPIO.setwarnings(False)
GPIO.setup(18,GPIO.OUT)
print "LED on"
GPIO.output(18,GPIO.HIGH)
time.sleep(1)
print "LED off"
GPIO.output(18,GPIO.LOW)
Once you have typed all the code and checked it, save and exit the text editor with “Ctrl + x” then “y” then “enter”.

Running the Code
To run this code type:

sudo python LED.py
