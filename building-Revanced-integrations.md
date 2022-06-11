# Building Revanced integrations

1. Make sure `$ANDROID_SDK_ROOT` or 
    `$ANDROID_HOME` is set correctly

2. Clone the repository

    ```
    git clone https://github.com/revanced/revanced-integrations && cd revanced-integrations   
   ```

3. Build the integrations

   ```
   ./gradlew build
   ```

The file will be located in `app/build/outputs/apk/release/app-release-unsigned.apk`

Rename the apk to integrations.apk

# Next Step

 [Building the ReVanced CLI](building-ReVanced-cli.md)
