# React Native

Following the great course [*The Complete React Native and Redux Course*](https://www.udemy.com/the-complete-react-native-and-redux-course) which created by [*Stephen Grider*](https://twitter.com/ste_grider).

The environment set up and initial steps is tested under Windows.

## Environment

1. Install [JDK](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html).
2. Install [Node.js](https://nodejs.org/) (bundled with npm).
3. Install [Python 2](https://www.python.org/).
4. Install [Android Studio](https://developer.android.com/studio/index.html).

## Initial Steps

1. Run `cmd`and `node -v` to check Node.js is installed.
2. Run `npm install -g react-native-cli`.
3. `mkdir` and `cd` to your working directory and run `react-native init projectname`.
4. **Android Studio Settings**
    1. After Step.3 is done, open *Android Studio -> Open an existing Android Studio project* to open your Anroid project, which is automatically created in Step.3.
    2. After opened, you'll see the error message like *"Failed to find target ..."*. Click on the *"Install missing ..."* hint to install the required SDK. (It's *v23* for the time being)
    3. After SDK installed, it'll show another error message like *"Failed to find Build Tools ..."*. Click on the *"Install Build Tools ..."* to install the required build tools. (Skipped Gradle plugin update after the installation is done.)
5. **Create Emulator**
    1. *Tools* -> *AVD Manager* -> *Create Virtual Device*, Choose *Nexus 5* should be fine.
    2. The default image will be latest one, please choose **Marshmallow** (API 23, x86_64 with Google API) to match with Step.4 installed SDK.
    3. Click on play button and it should work.
6. **Set Environment Variables (For Windows)**
    1. `JAVA_HOME` = `C:\Program Files\Java\jdk1.8.0_171` (change to your own version)
    2. Added `C:\Users\username\AppData\Local\Android\Sdk\platform-tools` to `PATH`
7. Re-run `cmd` with Administrator, `cd` to your working directory.
8. Run `react-native run-android` and the app should be installed and opened in the emulator. (The emulator must be opened before running the command.)

## Options

### Run AVD directly

1. List all of your AVD through `C:\Users\UserName\AppData\Local\Android\Sdk\tools\bin\avdmanager.bat list avd`, change **UserName** to your own user name.
2. Run `C:\Users\UserName\AppData\Local\Android\Sdk\emulator\emulator.exe -avd AVD_DEVICE_NAME`, change **AVD_DEVICE_NAME** to your own AVD device name, ex: Nexus_5_API_23

### Install ESLint for VSCode

1. Install [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) in [VSCode](https://code.visualstudio.com) market.
2. Run `npm install -g eslint` to install [ESLint](https://eslint.org) through npm.
3. Run `npm install --save-dev eslint-config-rallycoding` to install [Rallycoding config](https://github.com/StephenGrider/ESLint-Rallycoding).
4. Create `.eslintrc` under your working directory and add `{ "extends": "rallycoding" }` into the file and it should work.
