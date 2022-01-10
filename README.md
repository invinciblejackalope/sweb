# SWeb - Android Simple Web Browser

Using Android Studio 2020.3.1.
Emulator: Pixel 2 API 32.
Some aspects of the browser have been deprecated in the newest version of Android Studio. No observed problems so far.

Main browser code is in /app/src/main/java/landau/sweb/MainActivity.java.
HTTP requests are logged in the variable `requestsLog`.
Currently HTTP requests are displayed in a new browser window upon turning off `isLogRequests`.
Plan to log to an external file (use code from ExceptionLogger).
