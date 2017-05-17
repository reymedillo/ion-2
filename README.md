This is a starter template for [Ionic](http://ionicframework.com/docs/) projects.

## How to use this template

*This template does not work on its own*. The shared files for each starter are found in the [ionic2-app-base repo](https://github.com/driftyco/ionic2-app-base).

To use this template, either create a new ionic project using the ionic node.js utility, or copy the files from this repository into the [Starter App Base](https://github.com/driftyco/ionic2-app-base).

### With the Ionic CLI:

Take the name after `ionic2-starter-`, and that is the name of the template to be used when using the `ionic start` command below:

```bash
$ sudo npm install -g ionic cordova
$ ionic start mySideMenu sidemenu
```

Then, to run it, cd into `mySideMenu` and run:

```bash
$ ionic cordova platform add ios
$ ionic cordova run ios
```

Substitute ios for android if not on a Mac.


## Setup dev environment (Android)

1. Download and install the [Android Studio](https://developer.android.com/studio/index.html).
2. Once installed, go to your Android SDK folder path which can be found in your **C:\Users\YourUserName\AppData\Local\Android\Sdk**
3. Download and unzip the [latest sdk tools](https://dl.google.com/android/repository/tools_r25.2.3-windows.zip).
4. Copy the folder **tools** to your **sdk folder**. If there's an existing folder on your sdk, remove it before copying the latest download. *Note: Do not overwrite, some of the files will conflict.*
5. Add the **adb** command to you environment variables: 
    * Go to environment variables, edit path and add **%ANDROID_HOME%/platform-tools**
    * Run command `adb devices`
    * ```
        List of devices attached
        BH90F98M4D      offline
        ```
    * If your device shows **offline**, remove your device and connect again, then run the command until a verification dialog will pop-up on your device to allow the pc to automatically connect your device.
    * Once done, run the adb command again and check if the device is connected, just as shown below.
    * ```
        List of devices attached
        BH90F98M4D      device
        ```

## How to run in browser

1. Clone develop branch
2. Go to clone folder and `npm install`
3. To run it, call `ionic serve` or `ionic serve --port PORT_NUMBER_HERE`

## How to run in Android Device

1. Clone develop branch
2. Go to clone folder and `npm install`
3. Add the android platform to the project using `ionic platform add android`
4. Go to **store/ folder** and copy the **debug-signing.properties** file to **platforms/android**
5. Connect your device to your computer, make sure you have the sdk tools installed.
6. To run it, call `ionic run android`
