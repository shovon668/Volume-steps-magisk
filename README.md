# Volume steps changer for magisk
___
## What is this mod? 
this is just a simple mod that allows you to change the volume steps of your device.
inspired by mods such as the xposed volume steps+ mod and custom roms alike i thought id give magisk a spin after being out of the android development scene for a while.

Currently this mod changes the in call volume steps to 14 (android default: 7) and the media volume steps to 30 (android default: 15), im currently working on a way for users to set the amount. codes almost done with that and after that i will attempt an aroma installer for ease of use
___

## How does it work? 
it works by using magisk system.prop to add two build prop lines
``` 
ro.config.vc_call_vol_steps=14
ro.config.media_vol_steps=30
```
___

# Requirements
+ magisk 13.0+
___
# Installation

for installation instructions check the xda thread - (will add soon)
# FAQ
+ __will this work on X device?__ 
   Since this just makes build.prop edits that every android should accept because of the code to accept theese is in the [AudioService.java](https://android.googlesource.com/platform/frameworks/base/+/master/services/core/java/com/android/server/audio/AudioService.java#624)
   
Any other questions just hop over to the xda thread - (will add soon) or leave a bug report on the repo ill do my best to help!


## TODO

- [ ] aroma installer package for easier custom props
- [ ] partner apk to change prop file after install