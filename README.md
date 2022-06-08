# ReVanced Documentation

Instructions to build and install ReVanced.

## 🖥️ Prerequisites

- [ReVanced Patches (revanced-patches-VER.jar)](https://github.com/revanced/revanced-patches/releases/latest)
- [ReVanced CLI (revanced-cli-VER.jar)](https://github.com/revanced/revanced-cli/packages/1446603)
- Youtube/Music APK (make sure to download the bundled version on APKMirror)
- A rooted device

## 📱  Installing on your device

Make sure to extract `base.apk` from downloaded YouTube bundled APKs with a decompression tool like `7zip` and `WinRar`.

You also need to download both ReVanced CLI and ReVanced Patches JARs.

Give root permission to `ADB` shell.

- ```bash
  adb shell su -c exit
    ```
  
  Get the `ADB` device ID.

- ```bash
  adb devices
    ```

  Run the CLI.

- ```bash
  java -jar revanced-cli-all.jar -a base.apk -c -d [ADB device id] -o revanced.apk -p revanced-patches.jar -r -t temp
    ```

## 📦 Building

- Extract base.apk from YouTube bundle
  1. Open the downloaded `apkm` file as zip.
  2. Extract base.apk

- Revanced CLI

  - Clone the ReVanced CLI repo

      ```bash
      $ git clone https://github.com/revanced/revanced-cli.git
      $ cd revanced-cli
    
      # If on Linux-based OS, make sure to give desired permissions.
      $ chmod +x ./gradlew

      $ ./gradlew build
      ```

  - Patching YouTube APK on device
  
- Integrations
  
  - Make sure `$ANDROID_SDK_ROOT` or `$ANDROID_HOME` environment variables are set correctly.

  - Clone `revanced-integrations` repo.

     ```bash
      $ git clone https://github.com/revanced/revanced-integrations.git

      $ cd revanced-integrations

      #If on Linux-based OS, make sure to give desired permissions.
      $ chmod +x ./gradlew

      $ ./gradlew build
      ```

- Patcher

  - Clone `revanced-patcher` repo.

    ```bash
    $ git clone https://github.com/revanced/revanced-patcher.git

    $ cd revanced-patcher

    # If on Linux-based OS, make sure to give desired permissions.
    $ chmod +x ./gradlew

    $ ./gradlew publish
    ```

- Patches
  
  - Clone `revanced-patches` repo.

    ```bash
    $ git clone https://github.com/revanced/revanced-patches.git

    $ cd revanced-patches

    # If on Linux-based OS, make sure to give desired permissions.
    $ chmod +x ./gradlew
    $ ./gradlew build
    ```
