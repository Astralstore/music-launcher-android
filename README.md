# Music Launcher Android

![Picture](app/src/main/res/mipmap-hdpi/ic_launcher_foreground.png)

Project for re-purposing your old mobile phone in to a mp3 player via a launcher. No root privileges required.

[For Demo, visit here](https://youtu.be/ik7YlZy_g8U)

## Problem Statement

The objective was to repurpose an old Android phone into an MP3/MP4 player. I went through numerous articles discussing the conversion of a phone into a dedicated music player, but they mainly focused on installing apps, radio functions, and so on. I came across some sources that suggested rooting the device and executing various Command Line Interface (CLI) commands, along with flashing the operating system. This process seemed quite laborious.

Then, an idea struck me. I developed a custom launcher that would automatically open my music app upon startup, achieving precisely what I desired. I utilize YouTube Music, which also provides in-app video functionality. By disabling the lock screen, I ensured that the phone consistently remained in music mode. This approach can be applied to any app if the requirements align with mine, and it can even be utilized in an entirely offline capacity if desired. Thanks to the phone's WiFi, I can download songs directly to the device's storage for offline usage.

## Steps to Build

- Download the project.
- Download Java 8 SDK [here](https://adoptium.net/temurin/releases/?version=8)
- Install the SDK and open the project folder and open the gradlew file using Terminal (Linux)
```sh
./gradlew
```
or double click on ```gradlew.bat``` if you're using windows.
- if all software and dependencies are install, open terminal and type
For Linux
```sh
./gradlew build
```
For Windows open Command Prompt
```sh
gradlew build
```
- Check if there any bugs. Mostly it will be related to sdk downloads.
- The output file will be on ```app/build/outputs/apk```
- Install it on your phone and set the default launcher to 'Music Launcher' and there you go. All set.

## Notes
- This project targets for Android 4 (Kitkat) until Android 11
- Go to app/src/main/res/values/strings.xml.
- Change property target_app's value to your music app's package name. You can get the the package name from Google Play Store. It will be in URL.

