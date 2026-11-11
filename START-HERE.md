# Undertone 3.2 — start here

Undertone is a private media studio with ten audio slots, a visual connection network, a media gallery, rotating backgrounds, the intent-led Teal Apparitions HUD and a built-in creator-source Guide tab.

**Undertone 3.2, build 9 includes the five starter recordings and expanded studio.** The iPhone installer requires your own Apple signing; the Android installer is signed. [RELEASE-NOTES.md](RELEASE-NOTES.md) and the verification record describe the actual completed checks and remaining limits.

Prepared **November 11, 2026 (America/Denver)**. The public guide shows download availability, and the release notes record the completed checks.

## New in 3.2

The updated studio restores the previous **large, soft portal vortex behind the audio cards**, while keeping the small central intent image and editable routes. It adds intent-led HUD color and motion with continuous visibility, a white 64-cell tetrahedral grid around the centered Core, balanced starting channel positions, **Clear links / Undo clear**, and **Capture image** for saving a PNG of the current HUD into Gallery. The separate Aether art layer has been removed.

Open **Studio**, **Gallery**, **Saved HUD** or **Guide** from the top navigation. The **Guide** tab keeps the two supplied playlists and five optional references together, with steps for importing a creator-provided MP3/WAV where one is offered. Read [CREATOR-SOURCES.md](CREATOR-SOURCES.md) for the verified references and availability limits.

Build 9 also changes channel-cover storage: picture bytes are saved separately from the mix settings, so changing volume or seeking does not rewrite the cover image. The update keeps the older saved record for recovery while migrating readable covers. Keep the existing app installed during the update and retain your original media files. Channel covers accept readable images up to **20 MB**.

## Five included recordings

A fresh installation of **Undertone 3.2, build 9** starts with the five recordings captured from the owner's assigned iPhone mix. All five titles appear immediately. The first time you press **Play** for a recording, the app prepares its private local copy before playback. That preparation happens on the phone; you do not need to upload or stream the track.

If you press **Pause** or **Clear** while a recording is preparing, its queued playback is canceled. It will not start later just because preparation finishes. Your own channel edits and saved mix remain in place when you update. The starter pack is applied only to a fresh installation, so an update does not replace an existing mix.

The five MP3s total about **88 MB** before app packaging. Exact app download sizes and hashes are included in the release verification record. Android also prepares decoded audio on disk: after all five tracks have been prepared, allow about **1.5 GB of additional private audio storage**, on top of the installed app and any installer you keep.

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

Use the public download buttons above. You can also download the complete friends ZIP and extract it first. Open the appropriate app file from Downloads or Files. This page is the installation guide; the IPA and APK are the actual app installers.

The starter package includes five recordings selected by the owner and the supplied artwork. Bundled recordings are publicly downloadable with the installer. Your own later imports, saved mix, intent text, gallery uploads and credentials belong to your local installation.

## Updating an existing installation

**Keep the current app installed.** Follow the update section for your platform before replacing it. On iPhone, use the same Apple signing account and app identity. On Android, use the publisher's update signed with the same certificate. Deleting the app or clearing its data can remove the local library.

If you used the older native iPhone app, open **Help (question-mark icon) → Native library** after updating. Your existing library and mix are preserved, and changes made there update the studio when you return. Keep your original media files until you have checked the update on your phone.

## Check a download

The package's `SHA256SUMS.txt` (provided with the release) lists the actual app-file hashes. These commands calculate a hash for comparison; they do not install anything:

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
