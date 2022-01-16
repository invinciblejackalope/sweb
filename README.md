# SWeb - Android Simple Web Browser

## Setup

Download [Android Studio](https://developer.android.com/studio). On Linux, you might also need to change ownership of the Android SDK home directory so that the SDK Manager can make changes:
```
sudo chown $USER:$USER $ANDROID_HOME -R
```

You may need to download SDK tools as well: go to Tools > SDK Manager > SDK Tools. It is most fool-proof to download all of the tools.
After the appropriate SDK tools are installed, the project should download dependencies and build automatically or with Build > Make Project.

Follow the instructions [here](https://developer.android.com/studio/run/emulator) to create an Android virtual device (AVD) that we can run the application on. Currently, the app has been tested on **Android Studio 2020.3.1** using **Pixel 2 API 32.** 

## Run

Select Run > Run 'app' > Pixel 2 API 32 and the emulator should pop up.

## Notes

Some aspects of the browser have been deprecated in the newest version of Android Studio. No observed problems so far.

Main browser code is in /app/src/main/java/landau/sweb/MainActivity.java.

HTTP requests are logged in the variable `requestsLog`.

Currently HTTP requests are displayed in a new browser window upon turning off `isLogRequests`.

Plan to log to an external file (use code from ExceptionLogger).

