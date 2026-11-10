# Install Undertone on Android

Use the release file `Undertone-Android.apk` on **Android 9 or later**. The APK supports the normal Android CPU architectures without choosing a separate download. You do not need an Apple Account, AltServer or your own signing key. These instructions were checked against official guidance on November 8, 2026.

Keep **Android System WebView and/or Chrome updated** on the phone. The studio interface uses the system WebView; the audio mixer runs in a native background service.

## Install the APK

1. Save the APK to the phone, extract the package if necessary, and open it from Downloads or Files.
2. If Android blocks installation from that source, follow **Settings → Allow from this source** for the browser or file manager that opened the APK. You can also search Settings for **Install unknown apps**. This permission belongs to the source app, not every app on the phone.
3. Return to the installer and tap **Install**, then **Open**. Afterward you may turn that source's installation permission off again. Google's path is **Settings → Apps → Special app access → Install unknown apps**; manufacturer labels vary. [Google's installation instructions](https://support.google.com/pixelphone/answer/7391672?hl=en).
4. Leave **Google Play Protect enabled**. If it offers to scan the unfamiliar APK, let it scan and read the result. If it blocks the app as harmful, stop and send the exact message to the person providing the build; do not disable protection to get around it. [Google Play Protect](https://support.google.com/android/answer/2812853?hl=en).
5. Open Undertone and follow [APP-GUIDE.md](APP-GUIDE.md). Start with one short file and a low device volume.

Work-managed, child-managed or protected devices may prohibit this installation route. Follow the device's applicable management policy. Some regions and Android releases also have developer-verification requirements; consult the [current Android verification guidance](https://developer.android.com/developer-verification) if that is the message you see. A generic APK guide cannot override those requirements.

## Install an update without clearing your library

Keep Undertone installed, open the newer APK, and accept **Update**. The publisher must retain the same package identity and signing certificate for an ordinary in-place update. Android compares the signatures; a different certificate will not update the existing installation. [Android signing documentation](https://developer.android.com/studio/publish/app-signing).

Do not uninstall Undertone or select **Clear storage / Clear data** to resolve a signature mismatch. That can erase imports and settings. Keep original media copies and ask for a correctly signed update. An APK's signing certificate verifies its update identity; it does not mean the APK has been approved by Google Play.

## Background playback and battery settings

Android audio runs in a native foreground playback service, with Play/Pause/Stop controls in its media notification. Recordings and generated tones continue independently of the visual WebView. The app pauses when headphones disconnect or it detects phone/communication mode. It does not request exclusive audio focus, allowing concurrent playback where the system and other app permit it.

First test playback with Undertone open. Then lock the phone for a short test and try the other media app you intend to use. Audio interruptions, calls, system audio policies and manufacturer battery controls can still affect playback; installing an APK does not guarantee uninterrupted mixing with every app.

If playback stops only after the phone sleeps, inspect Undertone's own app battery settings. On Pixel, look under **Settings → Apps → App battery usage → Undertone → Allow background usage**. Keep normal optimization unless a playback problem calls for changing Undertone's setting. [Google's battery settings](https://support.google.com/pixelphone/answer/6090599).

On Samsung, **Settings → Apps → Undertone → Battery** may offer **Unrestricted**. Also check **Battery → Background usage limits** for Sleeping or Deep sleeping apps. Make any exception for Undertone specifically; settings vary by model. [Samsung's audio troubleshooting](https://www.samsung.com/us/support/troubleshoot/TSG10001337/), [Samsung's application-management guide](https://developer.samsung.com/mobile/app-management.html).

## Troubleshooting

- **“App not installed” / incompatible package:** confirm the complete APK downloaded, enough storage is available and your phone meets the release's requirements. Compare the file against `SHA256SUMS.txt`. Keep the exact error for troubleshooting.
- **“Conflicts with an existing package”:** check whether the installed copy came from a different signing key. Obtain the matching update; do not erase the existing library as a first step.
- **Install control unavailable:** check the source-app permission and device-management restrictions. Keep Play Protect enabled.
- **Import fails:** download the media fully onto the phone first, then select it again. An MP3/WAV filename does not guarantee a valid decodable file. For gallery video, both duration and codec must be supported.
- **Sound stops after Force stop:** open Undertone and start playback again. Force stop ends the running app; it is not a pause control.

Read [APP-GUIDE.md](APP-GUIDE.md) for channel controls, the gallery and the visual network.

## Audio storage on Android

The Android build accepts mono or stereo MP3/WAV imports up to **1 GiB per encoded file**. It decodes audio to local 48 kHz stereo PCM on disk, with a **4 GiB decoded-file cap** (about 3.1 hours). This uses roughly **1.4 GB of storage per hour of audio**, so long recordings need substantial free space even when the MP3 is small. The temporary encoded import is removed after decoding; retain your original files elsewhere. Android manages audio through the ten studio slots; the separate legacy **Native library** screen is an iPhone feature.
