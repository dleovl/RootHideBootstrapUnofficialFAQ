# **UNOFFICIAL** RootHide Bootstrap FAQ

DO NOT UPDATE YOUR PHONE NO MATTER WHAT!
SpringBoard tweaks *DO NOT WORK* currently. Tweak daemons do not work either.

Always remember, **DO NOT INSTALL `.TIPA` BUILDS FROM OTHER PEOPLE.** You risk installing malicious code if the code used to build the tipa is open source (meaning anyone could've modified the tweak to be malicious) and you're potentially installing outdated Bootstrap versions which may not function properly nor will they recieve support.
Don't run `rm -rf /var/`, it doesn't give you SpringBoard injection.

[Join the RootHide Discord server](https://discord.com/invite/scqCkumAYp)!
If you have an issue that isn't listed here, check the [issues](https://github.com/RootHide/Bootstrap/issues). If it's still not there, ask in the [Discord](https://discord.com/invite/scqCkumAYp). If you have something you'd like added here, let @dleovl in the server know, or make a PR in this repo.
This FAQ README will be consistently updated along with the [Bootstrap README fork](https://github.com/dleovl/Bootstrap/blob/main/README.md).

## Do I need TrollStore for this bootstrap?
YES! No TrollStore = Unsupported. No ifs, ands, or buts.
If you are on a supported version to install TrollStore, use [this guide](https://ios.cfw.guide/installing-trollstore/) to install TrollStore.

## How do I build the RootHide Bootstrap? (No PC/Mac required)
Check [here](https://discord.com/channels/1130859165942829106/1130859166488076331/1190488974528106607) for building with GitHub actions (must be in the Discord). This doesn't automatically update to the latest commit when a new one comes out, so you'll need to sync forks every time a commit is made. **DO NOT** rely on other peoples `.tipa` files as they can be outdated or malicious. Completely automatic building has been achieved by me and will be merged into the official repository when the developer sees fit.

Got a Mac and wanna use XCode? [Use this README](https://github.com/dleovl/Bootstrap/blob/main/README.md).

## Building doesn't work / I have a question about converting tweaks:
[Check my fork of the README](https://github.com/dleovl/Bootstrap/blob/main/README.md)

## Notifications are broken / apps keep asking for permissions!
Check out [issue #2](https://github.com/RootHide/Bootstrap/issues/2), this issue is already known. Disable and enable tweak injection to temporarily fix issue until next reboot.

## Cask 3 doesn't save settings!
Install [this fixed .deb](https://cdn.discordapp.com/attachments/1153426136802529280/1190903773606973470/com.ryannair05.cask3_1.0.2_iphoneos-arm64e.deb) with Sileo (pre-converted) (you may need to be in the Discord server for it to load)

## Cask doesn't work in Discord / other apps
These apps will need to be dumped, decrypted, and have an unsandbox entitlement like `get-task-allow` to allow the tweaks like Cask 3 to work. If this is too technical, ask in the Discord.

## How do I uninstall the Bootstrap?
Disable EVERY app in AppEnabler in the Bootstrap app. Reboot. Open the Bootstrap app and press uninstall. Thanks for staying with us!

## Why does the bootstrap say wait for fix? (test UI)
You are using an outdated leaked build. Please refer to the pin for proper instructions on how to update your bootstrap.

## DELETE ZEBRA!
It doesn't work well with rootless, please stick to Sileo. You can use whatever package manager you want, but if you have issues with installing packages in Zebra, it's because you're using Zebra. Switch to Sileo.

## What tweaks are supported?
Look for rootless tweak lists, and rule out the tweaks that require SpringBoard injection or daemons. These should work 99% of the time. Don't bother asking for Bootstrap-compatible tweak lists as you can easily tell which tweaks are supported or not, especially with the upcoming addition of SpringBoard injection., don't leave clutter everywher!

Keyboard-related tweaks and SnowBoard UI extensions (and ONLY UI extensions, NOT homescreen theming) work when you enable the app you want tweaked in AppEnabler.

## How do I update the Bootstrap?
Currently, for updating between beta versions, you may have to uninstall your bootstrap before updating. You can export sources and tweaks in Sileo, and backup your preferences through Filza to make this process easier. There is currently no known fix to this issue.

Uninstall, install your new `.tipa`, reboot, and bootstrap.

## No Sileo URL scheme?
Currently disabled for detection purposes. Copy repo URLs manually.

## 'Not a rootless package' in RootHide Patcher
Make sure the package is rootless (not already a RootHide tweak). For rootful, use the first option in the Patcher instead.

## Known broken tweaks (you won't get support)
iCleaner (Pro), as this software has a lot to do with daemons.

## How do I change tweak settings?
Use TweakSettings by CreatureSurvive on https://creaturecoding.com/repo/ and respring for it to show up, it's an app. If Settings works for you with tweak injection and you can see your tweaks in the app, you don't need TweakSettings. If TweakSettings works for you, you don't need Settings. To test settings, install PreferenceLoader and showtouch and enable com.apple.Preferences in Bootstrap AppEnabler. If you experience crashes with Settings after testing this, and you're sure no other tweak interferes with this, comment your device and iOS version [here](https://github.com/RootHide/Bootstrap/issues/37).

## Why does anti-detection not work 100%?
If you installed Filza through TrollStore, replace it with the [no URL scheme version](https://tigisoftware.com/download/Filza_NoURLScheme_4.0.0.ipa). If it still doesn't work, you may need to clear app data with Apps Manager by TIGI Software or uninstall/reinstall the app. If it STILL doesn't work, comment the application you're using along with a link to it and how to reproduce the warning (do you need to login/do anything beforehand) in [RootHide issue #48](https://github.com/RootHide/Bootstrap/issues/48).

## How do I disable OTA updates (working on even 17.0)
Turn off automatic updates in Settings, both iOS updates (installing and downloading) and security responses & system files.

Download the [Cowabunga IPA](https://github.com/leminlimez/Cowabunga/releases/download/v10.3.2/Cowabunga.ipa) and install with TrollStore.
Open and go to Tools > Miscellaneous and turn Supervised *ON*. Open Settings app and change the phones date to December 1st 2023.
Install the tvOS profile with [this .mobileconfig](https://betaprofiles.dev/dl/block-ota/BlockOTA_17.mobileconfig) and reboot. Disable Supervision from Cowabunga and set the date back to normal.

## Can I use JIT?
JIT by default works with applications specifically made to support JIT provided by TrollStore, but you can enable JIT for outdated applications by using the bootstrap if you don't want to inject with [TrollStoreJitEnabler](https://github.com/Rednick16/TrollStoreJitEnabler). Enabling injection into applications that require JIT with AppEnabler will allow JIT to be utilized.

## Why don't my apps say 'Open' in the App Store?
Applications injected in AppEnabler will not show up in the App Store. **DO NOT** click the cloud download button unless you know what you're doing or it's a 100% last resort.

To get it to say 'Open' again, disable injection in AppEnabler, and refresh icon cache in TrollStore.
