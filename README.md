# SWeb - Android Simple Web Browser

Using Android Studio 2020.3.1.

Emulator: Pixel 2 API 32.

Some aspects of the browser have been deprecated in the newest version of Android Studio. No observed problems so far.

Main browser code is in /app/src/main/java/landau/sweb/MainActivity.java.

HTTP requests are logged in the variable `requestsLog`.

Currently HTTP requests are displayed in a new browser window upon turning off `isLogRequests`.

Plan to log to an external file (use code from ExceptionLogger).

# Setup

Download [Android Studio](https://developer.android.com/studio). On Linux, you might also need to change ownership of the Android SDK home directory:
```
sudo chown $USER:$USER $ANDROID_HOME -R
```

You may need to download SDK tools as well: go to Tools > SDK Manager > SDK Tools (you may want to just download all of the tools). 
The project should download dependencies and build automatically. 

# Emulate the built application

Follow the instructions [here](https://developer.android.com/studio/run/emulator) to create an Android virtual device (AVD) and then run the app on the created device. 
