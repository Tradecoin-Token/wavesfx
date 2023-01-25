# WavesFX

![img](package/wavesfx_readme.png)


WavesFX is an open-source [Waves](https://wavesplatform.com) wallet for Windows, macOS and Linux.

[Telegram Chat](https://t.me/wavesfxchat)

Releases can be found on the [release](https://github.com/wavesfx/wavesfx/releases) list.


# How to build WavesFX

## 1. Prerequisites

### Install Java Development Kit (JDK) 16

[OpenJDK](https://jdk.java.net/16/) and [AdoptOpenJDK](https://adoptopenjdk.net/archive.html) are excellent choices. 

## 2. Obtain Source Code

```
git clone github.com/wavesfx/wavesfx
cd wavesfx
```
## 3. Compilation and packaging
### Build binary package
```
./gradlew jpackageImage 
```
Package will be located in `build/jpackage`   
### Build installer
**Note:** Wix, a third-party tool, is required to generate an installer for Windows.
```
./gradlew jpackage
```
# Bug Reports
Please use the issue tracker provided by GitHub to send bug reports or feature requests or join WavesFX on [Telegram](https://t.me/wavesfxchat)

# Edit Exe Name under build.gradle 
imageName = "YourOwnFork"
installerName = 'YourOwnFork'

Replace Wallet name under WavesFX.java "WavesFX Wallet"

..\src\main\java\com\wavesfx\wavesfx\logic\Waves.java line 13 to change Display Name
