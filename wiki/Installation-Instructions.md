To install the app on your android device or emulator, go to the [releases directory](https://git.uwaterloo.ca/s26nadee/cs346-project/-/tree/main/releases) and download the latest apk file (directly from the link or transfer it to your device). Then, to install it on your physical android device, simply select the apk file in your Files app to open a prompt to install the device and select "Install" (If not already done, you will have to change your settings first to allow your device to install unknown apps from this source). To install it on your emulator in Android Studio, you can drag the apk file from your file explorer onto the virtual device in Android Studio while the virtual device is running.

The server has been deployed on GCP (Google Cloud Platform) and the server's IP address has been set on the application so the app should automatically be able to communicate with the server (without any additional work) once it is installed.

**Note:** The app was tested on the following devices:
- Virtual Devices:
    - Google Pixel 3a, Android 14 (API 34)
- Physical Devices:
    - OnePlus 9R, Android 11
    - Samsung S22 ultra, Android 13