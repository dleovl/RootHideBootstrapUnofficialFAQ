**UNOFFICIAL** RootHide Bootstrap FAQ:

DO NOT UPDATE YOUR PHONE NO MATTER WHAT!
This bootstrap is currently unsupported on A15+ devices running iOS 17.0.
SpringBoard tweaks *DO NOT WORK* currently. Daemons do not work either.

[Join the RootHide Discord server](https://discord.com/invite/scqCkumAYp)!
If you have an issue that isn't listed here, check the [issues](https://github.com/RootHide/Bootstrap/issues). If it's still not there, ask in our [Discord](https://discord.com/invite/scqCkumAYp). If you have something you'd like added here, let @dleovl in the server know, or make a PR.
This FAQ README will be updated along with the [Bootstrap README fork](https://github.com/dleovl/BootstrapREADME/blob/main/README.md).

## Do I need TrollStore for this bootstrap?
YES! No TrollStore = Unsupported. No ifs, ands, or buts.
If you are on a supported version to install TrollStore, use [this guide](https://ios.cfw.guide/installing-trollstore/)

## How do I build the RootHide Bootstrap? (MAC NOT REQUIRED)
Check [here](https://discord.com/channels/1130859165942829106/1130859166488076331/1190488974528106607) or [here](https://discord.com/channels/1130859165942829106/1153426136802529280/1190424145327038554) for building with GitHub actions (must be in the Discord)

Got a Mac and wanna use XCode? [Use this README](https://github.com/dleovl/BootstrapREADME/blob/main/README.md).

## Building doesn't work / I have a question about converting tweaks:
[Check my fork of the README](https://github.com/dleovl/BootstrapREADME/blob/main/README.md)

## Notifications are broken / apps keep asking for permissions!
Check out [issue #2](https://github.com/RootHide/Bootstrap/issues/2), this issue is already known. Disable and enable tweak injection to temporarily fix issue until next reboot.

## Cask 3 doesn't save settings!
Install [this .deb](https://cdn.discordapp.com/attachments/1153426136802529280/1190903773606973470/com.ryannair05.cask3_1.0.2_iphoneos-arm64e.deb) with Sileo (pre-converted) (you may need to be in the Discord server for it to load)

## How do I uninstall the Bootstrap?
Disable EVERY app in AppEnabler in the Bootstrap app. Reboot. Open the Bootstrap app and press uninstall. Thanks for staying with us!

## Why does the bootstrap say wait for fix? (non A15+ iOS 17 / test UI)
You are using an outdated leaked build. Please refer to the pin for proper instructions on how to update your bootstrap.

## DELETE ZEBRA!
It doesn't work well with rootless, please stick to Sileo. You can use whatever package manager you want, but if you have issues with installing packages in Zebra, it's because you're using Zebra. Switch to Sileo.

## What tweaks are supported?
Look for rootless tweak lists, and rule out the tweaks that require SpringBoard injection or daemons. These should work 99% of the time. Don't bother asking for Bootstrap-compatible tweak list as you can easily tell which tweaks are supported or not.

## How do I update the Bootstrap?
Reboot, install the new .tipa like normal, rebootstrap.

## No Sileo URL scheme?
Disable for detection purposes.

## 'Not a rootless package' in Patcher
Make sure the package is rootless (not already a RootHide tweak). For rootful, use the first option in the Patcher.

## Known broken tweaks (you won't get support):
Flex 3 (not flex/FLEXing), iCleaner (Pro), Orion (iOS 17.0+)

## How do I change tweak settings?
Use TweakSettings by CreatureSurvive on https://creaturecoding.com/repo/ and respring for it to show up, it's an app. If Settings works for you with tweak injection and you can see your tweaks in the app, you don't need TweakSettings. If TweakSettings works for you, you don't need Settings. To test settings, install PreferenceLoader and showtouch and enable com.apple.Preferences in Bootstrap AppEnabler. If you experience crashes with Settings after testing this, and you're sure no other tweak interferes with this, comment your device and iOS version [here](https://github.com/RootHide/Bootstrap/issues/37).

## Why does detection not work 100%?
If you installed Filza through TrollStore, replace it with the [no URL scheme version](https://tigisoftware.com/download/Filza_NoURLScheme_4.0.0.ipa). If it still doesn't work, you may need to clear app data with Apps Manager by TIGI Software or uninstall/reinstall the app.
