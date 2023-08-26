# Development Setup
---


## Android Studio

If you have not already installed Android Studio, please do so now. You can get it here:

[Android Studio](https://developer.android.com/studio)

## Clone the Repository
First you need to check out the repository:

`$ git clone https://github.com/newhinton/Round-Sync`


Alternatively, you can use this url to check out the project via android studio.

`https://github.com/newhinton/Round-Sync`

You can do so by opening:

File>New...>Project from Version Control

After the Project was imported, you can start coding!
When you are ready to build your app to run it on your device or emulator, the build-process will build the app, and rclone. For this you need a working `go`-installation.

## Go

Follow the instructions here: [Install Go](https://go.dev/learn/)

You will also need to set up the environmental variables so that the go-executable can be found in `GOPATH`.

## NDK

To embedd the rclone-binary in the app, you will need the ndk. Please install it via Android Studio in the correct version.

The `gradle.properties`-file contains some definitions you might need for this.

This specifies the used NDK-version:

`de.felixnuesse.extract.ndkVersion=25.2.9519653`

## Rclone

When this app builds, it automatically builds rclone aswell. For that it is nessessary that you set up Go and the NDK beforehand.

If you want to use a different version of rclone to be build, you can edit the `gradle.properties`-file:

`de.felixnuesse.extract.rCloneVersion=1.63.1`

If you did not set up the ndk or go properly, the logs will tell you.


You are now done! Enjoy!
If you think this documentation is lacking, you can always make suggestions or change it. In the top-right is a pen-icon which lets you do so. Thanks!