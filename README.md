RaspiNotifier
=============

Python script that works with the Raspberry Pi's RPi.GPIO library in order to give physical LED notifications for multiple services.

This script pulls from various existing scripts/tutorials:
<ul>
<li><a href="http://learn.adafruit.com/raspberry-pi-e-mail-notifier-using-leds">Adafruit Learning System</a></li>
<li><a href="https://learn.sparkfun.com/tutorials/raspberry-pi-twitter-monitor">SparkFun</a></li>
</ul>

Setup:
======
In case you're completely new to Raspberry Pi, or just using its GPIO functionality, you will need several things first:
<ul>
<li>RPi Update: sudo apt-get update
<ul><li><i>If you've just updated your Pi, ignore this step</i></li></ul></li>
<li>RPi.GPIO: 
<ul><li>sudo pip install RPi.GPIO</li>
    <li><i>This is the key library that lets you progrom the serial pins on the RPi</i></li></ul></li>
<li>Python Controllers:
<ul><li>sudo apt-get install python-dev</li>
    <li>sudo apt-get install python-pip</li></ul></li>
<li>Python update (just in case):
<ul><li>sudo easy_install -U distribute</li></ul></li>
<li>Feedparser: 
<ul><li>sudo pip install feedparser</li>
    <li><i>This library parses the Gmail feed object returned</i></li></ul></li>
<li>Twython: 
<ul><li>sudo pip install twython</li>
    <li><i>This library uses the Twitter API for python</i></li><ul></li>
</ul>
<ul>
<li>Hardware:
<ul><li>Theres a few routes you can go in order to hook up LEDs to your RPi serial pins. Adafruit sells a Pi Cobbler breakout board and serial ribbon cable for under 10 bucks; but I went with a handfull of female-to-male jumper cables to a breadboard, since it was my first experiment and I could move things around easier</li></ul>
</li></ul>

Usage:
=======
After all that, run the RaspiNotifier.py as:
<ul><li>sudo ./RaspiNotifier.py</li></ul>

The Big Picture
===============
This project was started, and ultimatly will end up, as an extension to the <a href="http://www.instructables.com/id/LED-Glass-Desk-v20/">LED Glass Desk 2.0</a>. The desk displays an array of LED animations underneath a glass desk, elvating the standard desk look and feel. My vision was to take that one step further, and giving those LED animations purpose.
<p>
What if the LEDs only animated, or had specific animations for, when I got a new email? A new meniton on Twitter? Or a message in Facebook? Not only would my desk look and feel awesome, but it would have both form and function, and become part of the <a href="http://en.wikipedia.org/wiki/Internet_of_Things">internet of things</a>!
</p><p>
That being said, this project is a step towards acheiving this ulitmate goal. And since this is very much a side project, all in good time.
</p>
