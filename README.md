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

Select Run > Run 'app' > Pixel 2 API 32 and the emulator should pop up. The app itself is called **SWeb Debug**.

## Logging HTTP requests

Currently, the app only logs the URL of each HTTP request.

With the browser open, click the button on the bottom-right of the screen to bring up an "actions" panel. Check the box "Log requests" in order to begin logging HTTP requests, and uncheck the box in order to stop logging requests. Upon unchecking the box, the list of URLs will be written to an internal file called sweb-http.log. This file cannot be accessed from the Files app; to view the list of requests, either install [Android Debug Bridge](https://developer.android.com/studio/command-line/adb) or uncomment the line `Log.i(TAG, url);` to log the URLs in Android Studio.

## Notes

Some aspects of the browser have been deprecated in the newest version of Android Studio. No observed problems so far.

Main browser code is in /app/src/main/java/landau/sweb/MainActivity.java.

Next goal: Appium integration using UIAutomator2. Following [this document](https://appium.io/docs/en/about-appium/getting-started/?lang=en) and [these samples](https://github.com/appium/appium/tree/master/sample-code/java/src).

