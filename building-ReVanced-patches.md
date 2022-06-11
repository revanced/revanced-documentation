#  Building the patches
1. Clone the repository

   ```
   git clone -b non-root https://github.com/revanced/revanced-patches && cd revanced-patches   
   ```

2. Publish the patches

   ```
   ./gradlew publish
   ```

The file will be located in ```build/libs/revanced-patches-VERSION.jar```

Rename the jar to revanced-cli.jar

# Next Step

 [Building the ReVanced integrations](building-Revanced-integrations.md)
