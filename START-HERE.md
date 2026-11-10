# Undertone Studio — start here

Undertone is a private media studio with ten audio slots, a visual connection network, a media gallery, rotating backgrounds and the preserved Teal Apparitions effect.

**The updated starter release is being prepared.** The iPhone installer will require your own Apple signing; the Android installer will be supplied signed. The current iPhone Studio was tested by its owner; the new bundled-recording release is still being prepared. Check your own device after installing. [RELEASE-NOTES.md](RELEASE-NOTES.md) lists the completed checks and remaining verification, and [RELEASE-VERIFICATION.json](RELEASE-VERIFICATION.json) contains the release record.

## Choose your phone

| Phone | File in this folder | Installation route |
| --- | --- | --- |
| iPhone with iOS 17 or later | `Undertone-iOS.ipa` | Sign and install using your own Apple Account through AltServer on Windows or Mac. Follow [IOS-INSTALL.md](IOS-INSTALL.md). |
| Android 9 or later | `Undertone-Android.apk` | Open the signed APK on your phone and approve installation for that file's source app. Follow [ANDROID-INSTALL.md](ANDROID-INSTALL.md). |

The release targets **iPhone 14, iPhone 14 Plus, iPhone 14 Pro and iPhone 14 Pro Max**, along with other supported iPhones running **iOS 17 or later**. Install the same IPA on these models; a separate model-specific download is not needed.

**Android requirement:** Android 9 or later with updated Android System WebView and/or Chrome.

An unsigned IPA cannot install by tapping it in Safari or Files. An IPA signed for someone else's devices is not a universal installer for friends. Each iPhone owner uses their own signing account; nobody needs to share an Apple password with the sender. Android recipients use the supplied signed APK without signing it themselves.

The free iPhone route needs periodic renewal. The installation guide explains the seven-day period and app quota. This kit is a direct sharing package, not an App Store, TestFlight or Google Play listing.

## Keep everything together

Use the public download buttons when the starter release is ready. You can also download the complete friends ZIP and extract it first. Open the appropriate app file from Downloads or Files. This page is the installation guide; the IPA and APK are the actual app installers.

The upcoming starter package will include five recordings selected by the owner and the supplied artwork. Bundled recordings will be publicly downloadable with the installer. Your own later imports, saved mix, intent text, gallery uploads and credentials belong to your local installation.

## Updating an existing installation

**Keep the current app installed.** Follow the update section for your platform before replacing it. On iPhone, use the same Apple signing account and app identity. On Android, use the publisher's update signed with the same certificate. Deleting the app or clearing its data can remove the local library.

If you used the older native iPhone app, open **Help (question-mark icon) → Native library** after updating. Your existing library and mix are preserved, and changes made there update the studio when you return. Keep your original media files until you have checked the update on your phone.

## Check a download

The package's [SHA256SUMS.txt](SHA256SUMS.txt) lists the actual app-file hashes. These commands calculate a hash for comparison; they do not install anything:

```powershell
Get-FileHash .\Undertone-iOS.ipa -Algorithm SHA256
Get-FileHash .\Undertone-Android.apk -Algorithm SHA256
```

On macOS:

```sh
shasum -a 256 Undertone-iOS.ipa
shasum -a 256 Undertone-Android.apk
```

A matching hash confirms that a file matches the supplied manifest; it does not prove device compatibility or replace signing. After installation, follow [APP-GUIDE.md](APP-GUIDE.md) for importing media and testing playback.
