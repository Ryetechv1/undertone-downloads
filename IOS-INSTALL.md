# Install Undertone 3.2 on iPhone

Use `Undertone-iOS.ipa` on an **iPhone with iOS 17 or later**, with **AltServer / AltStore Classic**. AltStore PAL is a different distribution route. The main installation steps were checked against the official sources on November 9, 2026 (Denver). The app file must be present in your package before starting.

The release targets **iPhone 14, iPhone 14 Plus, iPhone 14 Pro and iPhone 14 Pro Max**, along with other supported iPhones running **iOS 17 or later**. Install the same IPA on these models; a separate model-specific download is not needed.

The 3.2 starter release includes five assigned MP3s totaling about **88 MB**. On a fresh install their titles appear immediately; first **Play** prepares each private local copy. Updating an existing installation keeps its assignments and saved mix. The release verification record provides the exact IPA size and hash.

## Before you start

Have the iPhone, its passcode, a USB data cable, an internet-connected Windows PC or Mac, the IPA, and access to **your own Apple Account** and any verification prompts. Enter account details only into the official signing software or Apple's authentication interface on your computer. Do not send them to the person sharing Undertone.

With Apple's free Personal Team provisioning, profiles expire after **seven days**. Apple permits **three installed development apps per device** and **ten App IDs within a seven-day period**. AltStore Classic itself occupies an installed-app slot. Direct AltServer installation avoids needing the AltStore app on the phone. [Apple account limits](https://developer.apple.com/help/account/basics/about-your-developer-account), [AltServer direct installation](https://faq.altstore.io/release-notes/altserver).

## Windows: prepare the computer

1. Download AltServer from [altstore.io](https://altstore.io/), extract its installer ZIP and run the included installer.
2. Follow AltStore's prerequisites for Apple-distributed **iTunes and iCloud**, not their Microsoft Store replacements. Official links: [iTunes 64-bit](https://www.apple.com/itunes/download/win64), [iTunes 32-bit](https://www.apple.com/itunes/download/win32), [iCloud installer linked by AltStore](https://updates.cdn-apple.com/2020/windows/001-39935-20200911-1A70AA56-F448-11EA-8CC0-99D41950005E/iCloudSetup.exe). These provide Apple components AltServer uses. If you already depend on Store iCloud, follow AltStore's documented alternate setup.
3. Start AltServer with **Run as administrator**. Approve the normal Windows prompt and allow its requested private-network access. Its icon appears near the clock, possibly under the hidden-icons arrow.

Source: [AltStore's Windows installation guide](https://faq.altstore.io/altstore-classic/how-to-install-altstore-windows).

## Mac: prepare the computer

1. Download current AltServer for Mac from [altstore.io](https://altstore.io/). Its current installation guide requires macOS 11 or later.
2. Move `AltServer.app` to Applications and open it. Look for its menu-bar icon.
3. Current AltServer does not require the old Mail plug-in. If an old copy requests one, update AltServer first; use the official legacy instructions only for a deliberately older setup.

Sources: [AltStore's Mac guide](https://faq.altstore.io/altstore-classic/how-to-install-altstore-macos), [AltServer release notes](https://faq.altstore.io/release-notes/altserver).

## Connect and install from either computer

1. Connect the unlocked iPhone by USB. Accept the computer-access prompt on your own computer and **Trust This Computer** on the iPhone; enter the phone's passcode there. Confirm the phone appears in iTunes on the Windows AltServer setup, or Finder on Mac. [Apple's trust instructions](https://support.apple.com/en-us/109054).
2. **Windows:** hold **Shift** while clicking AltServer's tray icon. **Mac:** hold **Option** while clicking its menu-bar icon. Select **Sideload .ipa…**, choose the iPhone when asked, and select `Undertone-iOS.ipa`.
3. Supply your own Apple Account in AltServer, complete any account verification it requests, and wait for its success notice. Keep the phone connected and unlocked during installation. Direct sideload is officially supported without first installing AltStore. [AltServer direct-sideload documentation](https://faq.altstore.io/release-notes/altserver).

## Authorize the first launch on iPhone

1. In **Settings → General → VPN & Device Management**, find the developer entry for **your own signing account**. Trust it and confirm the prompts. Older iOS versions may use “Profiles & Device Management.” This is the app's developer trust step, distinct from trusting the USB computer. [AltStore's trust instructions](https://faq.altstore.io/altstore-classic/how-to-install-altstore-macos).
2. In **Settings → Privacy & Security → Developer Mode**, enable Developer Mode, restart when requested, and confirm **Enable / Turn On** after restart using the device passcode. Apple may show this setting only after a development install or device pairing has been initiated. [Apple's Developer Mode guide](https://developer.apple.com/documentation/xcode/enabling-developer-mode-on-a-device).
3. Open Undertone and confirm **Studio / Gallery / Saved HUD / Guide** appear. Start with a low device volume and try one included recording using [APP-GUIDE.md](APP-GUIDE.md). Existing users can also check **Help → Native library** without deleting the installed app.

Developer Mode and developer trust authorize a development-signed app. They are not background-audio permissions. There is no special SoundCloud-style iOS permission that guarantees playback over every other app.

## Renew free signing before it expires

For the direct method, repeat **Sideload .ipa…** with the same IPA and signing account before the seven-day period ends. Install over the existing Undertone; do not delete it first. Set your own reminder before day seven. An expired app needs renewed signing before it will open again. [AltServer renewal requirement](https://faq.altstore.io/release-notes/altserver).

### Optional: manage refresh through AltStore Classic

1. In the ordinary AltServer menu, choose **Install AltStore → your iPhone** and sign with the same account. Complete trust and Developer Mode if needed.
2. For wireless refresh, enable the phone's Wi-Fi sync in iTunes on Windows, or **Show this iPhone when on Wi-Fi** in Finder on Mac. Apply the setting. Keep AltServer running on a computer reachable from the phone; a USB connection is also usable. [Windows setup](https://faq.altstore.io/altstore-classic/how-to-install-altstore-windows), [Mac setup](https://faq.altstore.io/altstore-classic/how-to-install-altstore-macos).
3. Save the IPA to Files on the phone. In AltStore Classic, open **My Apps**, use its **+** import action and choose that IPA. The official app's import action opens an IPA document picker. [AltStore import implementation](https://github.com/altstoreio/AltStore/blob/develop/AltStore/My%20Apps/MyAppsViewController.swift).
4. Use **My Apps → Refresh All** while AltServer is reachable. Check the displayed expiry instead of assuming background refresh succeeded. [AltStore refresh guide](https://faq.altstore.io/altstore-classic/your-altstore).

## Update while keeping the old library

Keep the existing Undertone installed and keep copies of your original media. Use the **same signing account, same signing tool and same app identifier** as your previous install; do not enable a duplicate-app or custom-identifier option. Install the newer IPA over it. An accepted in-place update keeps the app's data container; changing signing identity can prevent that update or create a separate app. Apple's update documentation describes preservation of Documents and Library data. [Apple's update-data guidance](https://developer.apple.com/library/archive/technotes/tn2285/).

The update preserves the older native iPhone library and mix. Open **Help (question-mark icon) → Native library** to check your recordings and make additional assignments. Choose **Return to Studio** when finished; the studio reflects those native changes. Audio continues to use the native player, while the new gallery and visual network have their own saved settings. Do not uninstall as the first response to an update error.

Build 9 stores channel-cover bytes in separate picture records and retains the legacy saved mix for recovery. Keep the existing app installed during that migration. After installing, verify that the recordings and channel pictures return, change a level, close and reopen the app, and confirm that the change remains saved. These are useful checks on each recipient's own phone; the release notes distinguish automated coverage from physical-device testing.

## Troubleshooting

- **Phone absent from AltServer:** unlock it, reconnect with a cable that carries data, try another USB port and confirm it appears in the Apple device-management software first. Charging alone does not prove a data connection. Use [Apple's device-detection guide](https://support.apple.com/en-us/108643).
- **Windows Apple component or sign-in error:** confirm the iTunes/iCloud prerequisites, start AltServer as administrator and inspect the exact error. Use the latest official installer and [AltStore troubleshooting](https://faq.altstore.io/altstore-classic/troubleshooting-guide). Do not apply random binary patches or share account details.
- **Internet drops when you plug in the iPhone / Wi-Fi icon becomes Ethernet:** keep the PC on its usual Wi-Fi and turn off **Personal Hotspot** on the iPhone while installing over USB. A USB hotspot can become Windows' preferred internet connection; an exhausted hotspot allowance can then interrupt Apple sign-in. USB device transfer and hotspot internet are separate. If you rely on the phone for your only internet connection, restore a working internet connection before signing.
- **“The provided anisette data is invalid”:** first restore a stable internet connection, check the PC's date/time, and update AltServer using the official download. Confirm the Apple-distributed iTunes/iCloud components are installed, then retry signing. This error concerns Apple authentication data. [AltStore's error reference](https://faq.altstore.io/altstore-classic/error-codes) covers errors 2013 and 3021. Use the current installer from the official AltStore website; the version available to you may differ from the publisher's earlier installation.
- **“Could not find AltServer”:** keep it running, use the same reachable private network, or connect USB. School/guest networks can isolate devices. Allow the specific AltServer firewall access instead of disabling the firewall. [AltStore connectivity guidance](https://faq.altstore.io/altstore-classic/troubleshooting-guide).
- **“Untrusted Developer” / Developer Mode required:** follow the two separate phone authorization steps above, then reopen the app.
- **Three-app or ten-App-ID limit:** free signing has separate quotas. Remove an unneeded app only after protecting its data, or wait for App IDs to expire. Repeatedly inventing new bundle IDs does not fix the quota. [Apple's limits](https://developer.apple.com/help/account/basics/about-your-developer-account).
- **App expires or update is rejected:** renew with the same account and identity. Keep the installed app and its data while investigating. A friend cannot fix your signing by sending an IPA signed with their personal account.

Once it opens, test one file in the foreground, with the screen locked, and alongside the other app you actually use. A successful computer installation is separate from successful playback on your phone.
