# Using the Revanced CLI
1. Connect your phone and copy ADB device name

```
    adb devices
```

2. Run the CLI

```
java -jar revanced-cli.jar -a youtube.apk -b revanced-patches.jar -m integrations.apk -o revanced.apk --sign -t cache -d {device id} -i microg-patch -i old-quality-layout -i amoled -i disable-create-button -i minimized-playback -i video-ads -i general-bytecode-ads -i seekbar-tapping --install
```

```
adb install revanced.apk
```

> A lot of patches require the integrations which you can merge by adding the -m flag and passing the integrations file as the argument.

> You can disable a patch by removing the patch name from the above command.

>You need to install Vanced MicroG in order to sign in into youtube. It is available on ApkMirror.