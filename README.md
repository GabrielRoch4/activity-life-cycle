# Activity Lifecycle Demo
This project is a simple Android application demonstrating the lifecycle of an Activity by overriding and logging key lifecycle methods. The application is designed to help understand how Android manages Activities in response to different user actions, such as opening, closing, minimizing, and rotating the app.

## Project Overview
In the MainActivity, the following lifecycle methods are overridden:

**onCreate()**
**onStart()**
**onResume()**
**onPause()**
**onStop()**
**onDestroy()**
**onRestart()**
Each method logs a message using Log.d() to display the current state in Logcat. Optionally, each state change is also shown as a Toast message for easier tracking directly on the screen.

## How to Test
Open the app – Observe onCreate(), onStart(), and onResume() in the logs.
Minimize and reopen – Check the calls to onPause(), onStop(), onRestart(), onStart(), and onResume().
Rotate the screen – Note how the lifecycle methods are called as the activity is recreated.
Close the app – Observe onPause(), onStop(), and onDestroy() as the activity ends.
