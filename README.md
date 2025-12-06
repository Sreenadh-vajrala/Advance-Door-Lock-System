# Advance-Door-Lock-System
This project that we built here is ADVANCED DOOR LOCKING SYSTEM with some basic operations. The major components include the Arduino UNO Board, LCD Display, Servo Motor (SG 90), I2C Connector along with LCD Display, Key pad(4x4), LEDs (2), Buzzer.
The Key Pad is what the user uses to enter the passcode or doing
any other operations specified in the locking system, and the LEDs represent the
currentstate of the door, if the door is locked then red LED glow and if it is open then
green LED glows. Buzzer is used for generating a sound when the user enters 3
incorrect passcodes or when user enters wrong old passcode while resetting the
passcode and the servo motor is a internal structure which is used for opening and
closing the door.
Once the system is initialized the display rolls a message “Enter # or * or A” on the
LCD display and upon pressing “*” we get to know about the overview of the
complete project and upon pressing “#” we get the display to enter the passcode
to unlock or lock the door and then upon pressing the “A” we get the display to
reset the passcode. The detailed functioning of each key is described below
1.When “*” key is pressed on the keyboard, the LCD Displays the complete
overview of the project which includes the name of the project, members of the
project and followed by the functions of the keys on the keyboard. The key that are
included are A-Resetting Passcode; B-Backspace; C-Clear; D-Home Screen; #-Entering the
passcode; * -Description; 0-9 digits -Numerical digits for 4- digit passcode.
2.When “#” key is pressed on the keyboard, the LCD asks to Enter the passcode,
once the correct passcode is entered the display shows CORRECT PASSCODE and
then servo motor starts rotating in a way to pull the knob and once the motor stops
the green led turn on and the red led turns off and the display shows a blinking
“DOOR UNLOCKED” message on the LCD display. But while entering the passcode
the user can use “B” key for clearing a single digit and “C” key for clearing the whole
4-digit passcode.
But when the entered passcode is incorrect then user still gets 2 more chances to
enter the correct passcode and still if the user enters the wrong passcode, then
after 3 wrong entries the buzzer starts generating the sound for 10 sec and also
displaying a message on the LCD display as “SECURITY ALERT”. The user can go to
main screen which displays the message “Enter # or * or A”.
3.When “A” key is pressed on the keyboard, the LCD screen displays “Resetting your
Passcode…” and then then it asks to enter the old passcode, once the correct old
passcode is entered the user gets a choice to change the passcode. The LCD displays
“Enter the new Passcode” and once entered, the passcode has changed and the LCD
displays a message “New passcode is changed successfully”.
But, while entering the old passcode, if the user enters it incorrectly then the buzzer
starts generating the sound for 5 sec and the LCD displays “SECURITY ALERT” and
goes back to the home screen.
Limitations:
when an unknown user tries to unlock the door while knowing the correct passcode,
the door automatically opens. We tried to add the fingerprint sensor which is like a
second step after entering the passcode to unlock or lock the door, but the sensor is
not working properly, we had to restrict ourself with the available resources and
compromise with security, and also with use of door knobs.
