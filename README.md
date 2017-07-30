# AdvanceHealthMonitoringApp

Part A:

Extend the basic app with the capability of creating a database for a patient. On entering the patient name, ID, age, and sex, the app should instantiate a database with table name Name_ID_Age_Sex. The table will have four columns: a) time stamp, b) x values, c) y values, and d) z values.

The app will then initiate a service that will connect to an accelerometer and collect data at a sampling frequency of 1 Hz. 

The data will be stored in the table with the time stamp of a sample and the raw three axes values of the accelerometer.

Whenever one hits the Run button the most recent 10 second data is pulled from the database and showed in the graph. The data is updated every second. When stop button is hit the graph is cleared.


Part B:

In this Part, we will extend Part A with the capability of uploading the data base to a web server.

Add another button to your UI named Upload Database. When you hit that button, your database should be uploaded to the web server.

Have another button in the UI named Download Database. When you hit that button the app should download data (if any) from the web server and plot the last 10 seconds of data in the graph.



INSTRUCTIONS:

Values of x, y and z from the accelerometer is coming in a range from -10 to +10. Therefore to smoothly show values of x, y and z on graph view, we have normalized their values from 0 to 20 on Y axis of the graph and 0 to 9 seconds for time on X-axis of the graph.

Downloaded database URI on device is(Nexus-5) :
***********************************************
/storage/emulated/0/databaseFolder/group22.db
***********************************************

same URI is used to save accelerometer values and group22.db is uploaded to the server with below URL :
*************************************************************
https://impact.asu.edu/CSE535Fall16Folder/UploadToServer.php
*************************************************************