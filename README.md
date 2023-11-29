# MAP-pd-7

This is the shared repository for an EDD class project.

Problem Statement:

Design Specifications:
A pill box and alarm system that will address the needs of dementia patients who may forget to take their medication. These specifications will outline what the solution must do and how it will work. Specifications are in priority order, with the most important goals listed first.

The system:

Notifies a user with dementia visibly and audibly that a pill has been detected in their pill box at a dose time
  Users can set two alarms per day for morning and night pill dosages
 

Uses a keyboard switch and Arduino to detect if a pill is in the box
  Padding on the inside of the lid will push a pill down on the keyboard switch
  If the switch is down (closed circuit), the pill is “on”
  If the switch is up (open circuit), the pill is “off”
  Detection, display, and alarm functions will be coded in Arduino IDE
  Arduino will process the input from the pill switch and a Real Time Clock (RTC) module to determine if an alarm will be triggered
 

Has 5 buttons wired to the Arduino to navigate the Liquid Crystal Display (LCD) and set alarms
  Arduino will display the real time and alarm-setting modes on an LCD
  "Switch" button to go between "Today's Date and Time" and "Set Alarms" display modes
  "Next" button to move between individual values of the settable dose clock and dose date in the "Set Alarms" menu
  Settable dose clock has hours and minutes in ##:## format and an option to change the dose date in months and days in ##/## format
  "Up" button moves a selected digit in dose clock up by one value
  "Down" button moves a selected digit in dose clock down by one value
  "Confirm" button, pressed to confirm a dose was taken and deactivate alarm
 

Alerts visibly and audibly that it is time to take a pill
  Arduino will provide alarm output through an LED and buzzer
  Activate the alarm if the pill is “on'' when the pre-set dose clock and real time clock match
  Deactivate the alarm if the pill is “off”
  Deactivate the alarm if the “confirm” button is pressed
  Alarm will reactivate if a pill is detected in the box five minutes after the "confirm” button was pressed
 

Is refillable and reusable
  Pill box is easy for elderly people to open
 

Alarm system, circuits, and computer are built into pill box
