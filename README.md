# Volume steps changer for magisk
___
## What is this mod? 
this is just a simple mod that allows you to change the volume steps of your device.
inspired by mods such as the xposed volume steps+ mod and custom roms alike i thought id give magisk a spin after being out of the android development scene for a while.

Currently this mod changes the in call volume steps to 14 (android default: 7) and the media volume steps to 30 (android default: 15), im currently working on a way for users to set the amount. codes almost done with that and after that i will attempt an aroma installer for ease of use.
___

## How does it work? 
it works by using magisk system.prop to add a build prop line
``` 
ro.config.media_vol_steps=30
audio.safemedia.bypass=true
```
___

# Requirements
+ magisk 19.0+
+ Android 9 or higher (Works on android 11!)
___

## Changelog
v0.1.1
- Added props to remove the safety "too loud" nagging message.
___

# Installation

for installation instructions check the xda thread - (will add soon)
# FAQ
+ __will this work on X device?__ 
   Since this just makes build.prop edits that every android should accept because of the code to accept theese is in the [AudioService.java](https://android.googlesource.com/platform/frameworks/base/+/master/services/core/java/com/android/server/audio/AudioService.java#624)
   
