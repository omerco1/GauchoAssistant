## Welcome to GauchoAssistant! 

Contributors: 
Omer Cohen, Jake Guida, Jake Bliss, Terrel Marshall

To run: 
Clone repo, open project in Android studio and login using your UCSB GOLD Credentials. 

 GauchoAssistant Manual
GauchoAssistant is a voice-controlled personal assistant application for UCSB students. It allows students to ask their android device basic questions pertaining to UCSB and receive a quick, accurate responses.
If it is the users first time opening the application, a login screen will be displayed. At the screen the student must enter their UCSB netid and password (please see notes at the bottom page regarding running the app).
The user will then be taken to a chat screen. The user can type a question using the field at the bottom of the screen. The user can also submit a question by clicking on the microphone icon in the upper right corner. The user will be prompted to ask a question verbally.
 
 The message will be displayed in the chat dialog. Once GauchoAssistant has found an answer to the question, it will respond and the answer will be displayed in the chat dialog.
Example commands:
“When is my next class?”
“What is on the menu for carrillo?” “What is the dinner menu for tonight?” “What are this quarter’s pass times?” “What is my pass time?”
If the user clicks on the setting icon in the upper left corner of the chat dialog, they can change the widget settings. These settings can be toggled on and off using the switches.
 
  On the user’s home screen, the widget will be displayed with the chosen settings. The user can resize the widget be dragging the upper or lower edge of the widget. The widget will display a certain subset of information depending on the size of the widget.
 
 A note to the grader:
- we utilize external memory to write specification files needed for UI integration. Thus if your scheduling information or widget preferences do not appear on the first run of the application, please close the app and run it once again. This rerun will allow these files to be initialized and properly registered with the program.
- Please ensure that you enter your password and username correctly as we do not implement any error handling for those fields. Entering login credentials incorrectly will cause our application to crash.
FURTHERMORE, THE APPLICATION MIGHT CRASH ON FIRST RUN. You might get a bug saying:
“ File not found: java.io.FileNotFoundException: /data/user/0/com.jakebliss.gauchoassistant.gauchoassistant/files/my_schedule.txt (No such file or directory)
2018-12-12 23:06:29.765 27151-27151/com.jakebliss.gauchoassistant.gauchoassistant D/AndroidRuntime: Shutting down VM
”
This means that our schedule data has not been initialized in your emulator. To fix do the following:
On your android studio:
View → Tools Windows → Device File Explorer
Within the uploaded zip file, locate “my_schedule.txt”, you need to upload this file to the /data/user/0/com.jakebliss.gauchoassistant.gauchoassistant/files folder.
Within Device File Explorer window, expand the “​data​​” folder, inside the data folder expand the “​data​​” (same named) folder. Once inside that folder, expand the “​com.jakebliss.gauchoassistant.gauchoassistant​​” folder, from there expand the “​files​​” folder. Inside that folder, right click “​upload”, t​​ hen upload the “my_schedule.txt” file from the uploaded zip file.
Re-run the application twice with entering your credentials to get the app to get on track with you scraped data.
