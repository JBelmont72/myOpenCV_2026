
Note the servo library is from laesson 19. minute 17
 https://www.youtube.com/watch?v=i7hMx6YLR0Q
 lesson 20 seervo with poteniometer https://www.youtube.com/watch?v=X6ZC-L02aEs&list=PLGs0VKk2DiYxdMjCJmcP6jt4Yw6OHK85O&index=23p

sunfounder tutorials! https://docs.sunfounder.com/projects/raphael-kit/en/latest/

sunfounder has the tutorials of PW and the code plus a lot more
https://github.com/sunfounder/raphael-kit/blob/master/python/ADC0834.py is for the adc0834,  check out the other codes as well.  



In this lesson we give you a step by step tutorial on how to create a low cost IP camera from a Raspberry Pi and the Raspberry Pi camera module.  (If you need to get a Raspberry Pi and Camera Module, we recommend this complete starter Kit, which you can order HERE.  If you already have a Raspberry Pi, and just need a camera, you can get the camera module HERE.) We are going to assume you already have your Raspberry Pi up and running, and are able to make a connection to it via Putty or SSH. If you are completely new to the Raspberry Pi, you should probably start with the  first two lessons on THIS PAGE.


https://toptechboy.com/tag/raspberry-pi/page/3/

This video will take you through the steps one at a time. In addition, the tutorial below has the commands that you can copy and paste. We recommend you both follow the video, and get the steps from the instructions below, so you do not have to manually type the commands. Be very careful . . . you must be precise in following these instructions for things to work.

OK, now assuming you have your Raspberry Pi up and running, and you can connect via Putty or SSH, These are the steps to get your dandy personal IP camera working. You will type or copy and paste these lines one at a time into the Raspberry Pi command line.

STEP 1: Get Your Raspberry Pi Up to Date:

sudo apt-get update
sudo apt-get upgrade
STEP 2: Install Lighttpd Web Server:

sudo apt-get install lighttpd lighttpd-doc php5-common php5-cgi php5 zip
STEP 3: Enable Server to Process PHP Scripts

sudo lighty-enable-mod fastcgi-php
sudo lighty-enable-mod cgi
sudo lighttpd-enable-mod fastcgi
STEP 4: Create a PHP WEB Page:

sudo nano /var/www/html/php.php
Now you will want to type or paste this info into the nano window.

<?php phpinfo(); ?>
STEP 5: Save your nano file with these key strokes:

Ctrl O
Enter
Ctrl X
To be clear, you press the Control key and the letter “O” at the same time. Then press the enter key. Then press the Control and “X” key at the same time.

STEP 6: Restart the Webserver:

sudo /etc/init.d/lighttpd restart
STEP 7: Check That the WEB Server is Working:

Go to a browser on a Windows computer on your network, and type:

http://10.1.15.94/

(NOTE: You would use your Pi’s IP address above. The number I use above is the IP address of our Pi. Your number will be different. You can find out your IP address on the pi by typing ifconfig into the terminal window.)

If you configured things correctly, you should get an Apache info page pop up.

this is the list of of the old Raspberry pi series:
https://toptechboy.com/raspberry-pi-with-linux-lessons/


Raspberry Pi Linux LESSON 26: This lesson shows how to control the GPIO pins on the Raspberry Pi using Python. We show how to select the pins, set their modes and then how to send them high or low.

Raspberry Pi LESSON 27: This lesson shows you how to simulate analog voltages on the Raspberry Pi GPIO pins using Pulse Width Modulation. This is like the  Arduino analogWrite function.Arduino sensors

Raspberry Pi LESSON 28: This lesson presents a step-by-step tutorial on how to simply control the position of a servo using the Raspberry Pi GPIO pins and Python.

Raspberry Pi LESSON 29: In this lesson we show how to set up the GPIO pins as inputs and how to read from them in python. We also show how to activate the internal pullup resistors on the GPIO pins. We demonstrate this with a simple circuit with two push buttons.

Raspberry Pi Lesson 30: In this lesson we show how to control two LEDs from two push buttons using Python. This requires us to use GPIO pins as inputs and outputs.

 Raspberry Pi Lesson 31: In this tutorial we show how to create a dimable LED whose brightness is controlled by two push buttons.

Raspberry Pi LESSON 32: Options for analog input to the Raspberry Pi.

Raspberry Pi LESSON 33: This lesson shows you how to boot the Raspberry Pi into the Graphical User Interface for a Windows Like user experience.

Raspberry Pi LESSON 34: Google Chromium is a version of Chrome that will run on the Raspberry Pi. This lesson shows you how to install this browser on your Raspberry Pi.

Raspberry Pi LESSON 35: This tutorial shows you how to install a free office-like word processor and spreadsheet onto your Raspberry Pi.

Raspberry Pi LESSON 36: This lesson shows you how to open programs, files and folders with a single click in the graphical user interface.

Raspberry Pi LESSON 37: This lesson shows you how remotely run a graphical user interface on the Raspberry Pi. Get the full windows like experience on a remote desktop.

Raspberry Pi Lesson 38: This lesson shows how to build an IP camera based on Raspberry Pi and the RPi Camera Module.

The Ultimate Raspberry Pi Project: To the edge of space and back with a Raspberry Pi! This project shows you just how far you can take a Raspberry Pi.

```h
Raspberry Pi Linux LESSON 26: This lesson shows how to control the GPIO pins on the Raspberry Pi using Python. We show how to select the pins, set their modes and then how to send them high or low.

Raspberry Pi LESSON 27: This lesson shows you how to simulate analog voltages on the Raspberry Pi GPIO pins using Pulse Width Modulation. This is like the  Arduino analogWrite function.Arduino sensors

Raspberry Pi LESSON 28: This lesson presents a step-by-step tutorial on how to simply control the position of a servo using the Raspberry Pi GPIO pins and Python.

Raspberry Pi LESSON 29: In this lesson we show how to set up the GPIO pins as inputs and how to read from them in python. We also show how to activate the internal pullup resistors on the GPIO pins. We demonstrate this with a simple circuit with two push buttons.

Raspberry Pi Lesson 30: In this lesson we show how to control two LEDs from two push buttons using Python. This requires us to use GPIO pins as inputs and outputs.

 Raspberry Pi Lesson 31: In this tutorial we show how to create a dimable LED whose brightness is controlled by two push buttons.

Raspberry Pi LESSON 32: Options for analog input to the Raspberry Pi.

Raspberry Pi LESSON 33: This lesson shows you how to boot the Raspberry Pi into the Graphical User Interface for a Windows Like user experience.

Raspberry Pi LESSON 34: Google Chromium is a version of Chrome that will run on the Raspberry Pi. This lesson shows you how to install this browser on your Raspberry Pi.

Raspberry Pi LESSON 35: This tutorial shows you how to install a free office-like word processor and spreadsheet onto your Raspberry Pi.

Raspberry Pi LESSON 36: This lesson shows you how to open programs, files and folders with a single click in the graphical user interface.

Raspberry Pi LESSON 37: This lesson shows you how remotely run a graphical user interface on the Raspberry Pi. Get the full windows like experience on a remote desktop.

Raspberry Pi Lesson 38: This lesson shows how to build an IP camera based on Raspberry Pi and the RPi Camera Module.

The Ultimate Raspberry Pi Project: To the edge of space and back with a Raspberry Pi! This project shows you just how far you can take a Raspberry Pi.

```

to access other PW tutorials shortcuts into toptechboy to avoid the archived lessons
https://toptechboy.com/create-a-dimable-led-with-a-potentiometer-on-the-raspberry-pi/

https://toptechboy.com/library-for-i2c-connection-of-the-lcd1602-to-the-raspberry-pi/

https://toptechboy.com/library-for-i2c-connection-of-the-lcd1602-to-the-raspberry-pi/

https://toptechboy.com/creating-a-programmable-temperature-alarm-with-the-raspberry-pi/

https://toptechboy.com/using-a-photoresistor-to-detect-light-on-the-raspberry-pi/#google_vignette

https://toptechboy.com/library-for-reading-a-16-button-keypad-on-the-raspberry-pi/

https://toptechboy.com/raspberry-pi-lesson-36-motion-detection-alarm-system-with-lcd-and-keypad/

https://toptechboy.com/raspberry-pi-lesson-37-raspberry-pi-security-system/#google_vignette
https://toptechboy.com/raspberry-pi-lesson-38-motion-detection-alarm-with-multiple-alarms/