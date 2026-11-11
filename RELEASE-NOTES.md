# Undertone 3.2, build 9 — release details

Prepared **November 11, 2026 (America/Denver)**. The iPhone automated checks,
Android complementary integration coverage and package verification below are
complete for these exact build 9 installers. Android acceptance combines the
listed checks from two runs of the **same signed APK**; it does not relabel the
partially completed run as a full single-run pass.

| Platform | Stable file | Exact bytes | Approximate download |
| --- | --- | ---: | ---: |
| iPhone | `Undertone-iOS.ipa` | 63,085,485 | 63.1 MB |
| Android | `Undertone-Android.apk` | 60,446,761 | 60.4 MB |

SHA-256:

```text
50a5f0edb3c169ff54f366974050d1c0093b643f5e6dfdfab6148abe98ae27e9  Undertone-iOS.ipa
bbb8d91c17cb84a4f2f943acbd1020b75eeeb828dfdb02e894984a910afe2f77  Undertone-Android.apk
```

The iPhone IPA is **unsigned**; each recipient signs with their own Apple
Account. Free signing needs renewal every seven days. On Windows, **Shift-click
AltServer → Sideload .ipa…** selects the file; the iPhone installation guide
contains the complete steps. The Android APK is signed with the publisher's
retained certificate for ordinary in-place updates. This is a direct download
kit, not an App Store, TestFlight or Google Play listing.

## iPhone automated and package checks

Run **42981816658**, source commit
**fb1a7d879d9709c51f27848e3f665912377dfa42**, completed successfully using
**Xcode 26.5 and the iOS 26.5 simulator runtime**:

- **169 shared tests** and **37 native unit/integration tests** passed.
- Both primary **iPhone 14 UI tests** and the **iPhone 14 Pro Max layout test**
  passed. Both reviewed sizes were readable and their cover images decoded.
- The new legacy-File regression recovered ten channel covers byte-for-byte,
  repeated production settings saves, recreated the WebView and decoded covers.
- The Gallery File regression checked restoration, resaving and WebView
  recreation without changing the Gallery storage format.
- Actual original-renderer HUD PNG capture and Gallery persistence passed.
- The Release arm64 archive passed. Package inspection verified CRC, app
  identity, iOS 17 minimum, unsigned state, all 18 shared web resources, the five
  exact original MP3s and the unchanged preserved HUD.

These are automated/simulator and package results. **Build 9 was not separately
installed or tested on a physical iPhone.** Each recipient can check playback
and saved settings on their own device using the supplied guide.

## Android static checks and complementary integration status

The signed build 9 APK passed **112 DSP cases**, **27 creator-link validation
cases**, archive/identity checks and APK Signature Schemes **v2/v3** verification.
Its retained signing certificate supports ordinary in-place updates. All **19
frozen packaged assets**, all five original MP3 hashes and the preserved HUD were
checked against the frozen source. The package is not debuggable.

Android integration acceptance combines these actual checks on the exact same
APK SHA-256 listed above:

- **42983219802** completed creator-link checks, native core, all ten legacy
  cover migrations, replacement-artwork and metadata reload, graph create/edit/remove/reverse
  checks and clean unobscured main-Flow screenshots reviewed for visual
  acceptance. These are the covered checks from that run, not a claim that the
  entire run completed successfully.
- **42984662083 passed the remaining focused integration suite:** Clear links /
  Undo clear persistence and reload; intent apply/reload, Cancel and remove;
  actual nonblank HUD PNG capture into Gallery and restoration after reload;
  foreground playback notification; same-Activity notification re-entry;
  advancing audio after Activity destruction; native WAV/MP3 playback; ten
  simultaneous voices; and limiter checks.

The combined coverage completes the Android visual and full-interface/background
acceptance for this installer. The verification record lists both run IDs, their
covered checks and the emulator-environment limits. No production APK change
separates those runs.

No physical Android phone was tested. Device-specific power controls, audio
interruptions and another app's behavior can affect playback; the installation
guide includes a practical recipient playback check.

## Channel pictures and the prior build 8 incident

Build 9 stores channel-cover bytes separately from the mix settings. Cover
images can be up to **20 MB** and must decode as readable images. The mix stores
artwork references instead of rewriting cover File/Blob objects on every level
or seek change. The legacy saved record is retained for recovery. An unreadable
individual cover keeps its recovery reference, shows fallback artwork and a
warning, while audio settings remain independent.

Build 8 had installed on the owner's iPhone running iOS 26.5.2, then reported
snapshot/settings-save errors and showed missing channel pictures. The original
native recordings remained listed and playable; private recovery inspection
found the ten channel JPEGs and intent PNG intact. That historical incident did
not establish audio loss. Build 9's recovery behavior now has the automated
File/IndexedDB coverage described above; that evidence is not relabeled as a
physical build 9 test.

The change isolates channel artwork. Gallery/video/background/intent storage
formats remain unchanged. No large-video memory migration is added. Gallery
still permits **50 items**, including **ten videos up to 90 seconds**, and the
background manager holds **five timed images or GIFs**.

## Studio features retained

The previous **large, soft portal vortex behind the audio cards** remains,
including the small central intent image and editable channel/Core/HUD routes.
The studio retains all ten audio slots, optional per-slot tone generators,
stereo pan/movement, the intent-led continuously visible Teal Apparitions HUD,
white 64-cell grid, Clear links / Undo clear, PNG HUD capture into Gallery,
Studio / Gallery / Saved HUD / Guide navigation, and removal of the separate
Aether art layer. Intent and routes organize the visualization and do not change
a recording's audio signal or establish a therapeutic outcome.

## Five exact original starter recordings

The same five recordings total **87,924,242 original bytes** before packaging.
Slot 1 is 24 minutes 24.764 seconds; slots 2–5 are 10 minutes 11.998 seconds each.
Slots 2–5 have distinct titles but byte-identical MP3 contents, deliberately
preserved at the owner's request. All five original hashes were checked in both
final installers; compression explains why the app download sizes differ from
the original MP3 byte total.

Fresh installs show all five titles immediately. First Play prepares a private
native copy. Pause/Clear cancels queued playback; an Android conversion already
running may finish caching. Existing mixes, edits and intentionally cleared
slots take precedence in an ordinary in-place update. The starter pack seeds
fresh installs only. Preparing all five on Android can add about **1.5 GB of
private decoded audio**, beyond the installed app and retained installer.

## Creator sources and local privacy

The Guide tab and [CREATOR-SOURCES.md](CREATOR-SOURCES.md) include the supplied
[download MAIN playlist](https://youtube.com/playlist?list=PLM1lay8BpiBA) and
[download playlist](https://youtube.com/playlist?list=PLcgtgh3iO-5g), plus five
optional titles from the second playlist. The playlist inspection is dated
**November 10 UTC**. Playlist ownership is not video-uploader identity;
per-video uploader identity and direct/free-file availability remain unverified.

Expand Details / description and creator-pinned comments. **Where the creator
provides a free MP3/WAV**, use their link and terms, save to Files / Downloads
and import into slots 6–10. A free stream or a YouTube offline save does not
establish an importable audio file. Creator titles do not establish health,
DNA, biological or metaphysical benefits.

Compatibility targets remain supported iPhones on **iOS 17+**, including the
**iPhone 14 family**, and **Android 9+** with updated Android System WebView
and/or Chrome. One IPA serves supported iPhones. No testing of every physical
model is claimed.

The public installers contain the five selected recordings and starting
artwork/assets. Later imports, Gallery uploads, channel covers, intent text and
saved mixes stay in the recipient's local app. Private backups, credentials,
pairing records and signing private keys are excluded from the sharing kit.
