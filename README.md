# Releaf
## IOS app for users to find eco-friendly art and designs they can make at home during COVID
* Basically, DayMax rings your custom ringtone when it's time to take medicines. You can set alarms, record your heart rate and health stats, and tell DayMax to notify your Primary Care Physician (PCP) in emergency!
* DayMax is portable - you can carry it around to work or school
* Low-cost + easy maintainence: Built under $5 dollar budget, battery can be recharged

<img src="https://www.awn.com/sites/default/files/styles/original/public/image/attached/1023010-big-hero-6-leftfullcomp.0025-1200.jpg?itok=W9pdebjv" width="1000" height="350">

# Installation Note
Before using DayMax, some settings for the email notification service must be configured.
1. Include ESP32 Mail Client library. In the Arduino IDE go to Sketch > Include Library > Manage Libraries. Search for "ESP32 Mail Client" by Mobizt, and install the library.
2. Close and restart the Arduino IDE.
3. If when compiling/uploading, you get an error of "#error: architecture or board not supported", go to the Arduino libraries folder in your local computer, then move/delete the entire "SD" folder from the libraries folder.  

If you want to remove all the email notification, comment everything on the email_notif.ino file and the code in final.ino that calls the email function (search "email").
