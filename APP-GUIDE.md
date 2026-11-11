# Use Undertone 3.2

The expanded studio combines ten audio slots with a visual network and a private media collection. The flow diagram and intent text are visual organization tools. They do not route audio signals, change a recording's contents or establish a subliminal, medical or therapeutic effect.

## Five included recordings

A fresh installation of **Undertone 3.2, build 9** starts with the five recordings captured from the owner's assigned iPhone mix. All five titles appear immediately. The first time you press **Play** for a recording, the app prepares its private local copy before playback. That preparation happens on the phone; you do not need to upload or stream the track.

If you press **Pause** or **Clear** while a recording is preparing, its queued playback is canceled. It will not start later just because preparation finishes. Your own channel edits and saved mix remain in place when you update. The starter pack is applied only to a fresh installation, so an update does not replace an existing mix.

The five MP3s total about **88 MB** before app packaging. Exact app download sizes and hashes are included in the release verification record. Android also prepares decoded audio on disk: after all five tracks have been prepared, allow about **1.5 GB of additional private audio storage**, on top of the installed app and any installer you keep.

## First listen

1. Lower your phone's output volume, open Undertone and allow the interface to finish loading.
2. Choose one of the five starting tracks and tap **Play**. Allow its first-use preparation to finish. To add your own file instead, select **Import audio** or an empty channel and choose an MP3 or WAV; download cloud-provider files onto the phone first.
3. **Pause** keeps the current position; **Stop** rewinds. Use the bottom transport to control the mix. Saved audio returns paused on a new launch.
4. Add more recordings, up to **ten slots**. A slot can hold a recording, a generated tone or both. Importing into an occupied slot replaces that slot's recording.
5. Tap a channel name or its controls button to adjust level, seek, mute, looping and stereo position. Optional automatic panning moves between its selected bounds.
6. Test the app with the phone locked and with your usual second media app before relying on a long background session. Calls, alarms, device controls and other apps can interrupt playback. Use the platform installation guide if background playback stops.

The top navigation opens **Studio**, **Gallery**, **Saved HUD** and **Guide**. On a narrow screen within Studio, **Flow**, **Channels** and **Media** switch workspaces. The bottom master transport remains available.

On Android, the native media notification also provides Play/Pause/Stop. Headphone disconnection and phone/communication mode pause playback. Long imports decode to disk and can use about 1.4 GB per hour; see the [Android storage limits](ANDROID-INSTALL.md) before importing a large collection. The iPhone version also uses native audio; the visual interface is not responsible for keeping audio running while the phone sleeps.

## Master level and generated tones

The master runs from **0% to 1,100%**. At 100% it adds no master boost; 1,100% represents 11 times nominal digital amplitude before output limiting. It cannot make the phone's amplifier 11 times stronger, and an already-loud recording may gain little extra loudness because the limiter contains peaks. Set comfortable device volume first, then adjust the mix gradually.

Each slot's optional tone has its own level, stereo controls and carrier frequency up to **20,000 Hz**. Carrier choices are sine, triangle, square, sawtooth, pulse, asymmetric, parabolic, sinc and fractal. Modulation changes the carrier's amplitude; it is separate from carrier frequency. Very high settings may be inaudible or limited by the phone and output device. No audible tone is not a reason to raise the output abruptly.

## Create and edit the visual network

The network has **12 endpoints**: **Core**, channels **1–10**, and **HUD**. Empty channels can participate; adding or clearing a recording does not delete their visual routes.

The previous **large, soft portal vortex** fills the center and extends behind the audio cards. Your optional intent image stays small at the center. The larger vortex keeps the existing intent editing and channel/Core/HUD routes available; its appearance does not change audio playback.

1. Tap the centered **Set intent / Edit intent** control to enter text and choose a color. You can also choose an intent image. The Core is surrounded by a fine white 64-cell tetrahedral grid; the grid is decorative and does not block connection controls.
2. Turn on **Link**, choose an origin port, then choose one or more destinations. The origin remains selected for branching. You can also drag between ports, including from the Core's connection button or port.
3. Core, channels and HUD can each be either origin or destination. **Both directions** in the connection dialog creates two directional links.
4. Tap a curve to edit it, reverse its direction or remove it. A reverse changes the visual link, not audio playback. When the reverse direction already exists, reversing merges into that existing direction instead of creating a duplicate.
5. Drag channel title bars to arrange the cards. The starting layout is balanced around the centered Core, with a centered Core ↔ HUD route. The **Fit view** icon, labeled **Reset card positions** for accessibility, restores the starting card positions and leaves your links intact.
6. Use **Apply to visualization** to keep dialog changes, or **Cancel** to discard them. Canvas edits begin saving after each change.
7. **Clear links** removes the visual routes only. **Undo clear** restores that cleared set without deleting routes you added afterward. It does not clear recordings or the saved intent. The undo action applies to the current Flow editing session, so restore before leaving or reloading if needed.

New networks start with Core → channels 1–5 and two-way HUD links to Core and all ten channels. These starting links are editable. The HUD links are added once when migrating an older graph; removed links stay removed on later launches.

In **Motion settings**, **Reverse vortex** changes the vortex's rotation and inward/outward movement. Speed, glow and visual pause are separate from link direction and audio transport. Pausing visuals does not pause the audio mix.

## Gallery: images, GIFs and videos

Open **Gallery** or the compact media panel, then use **Add media**.

- Up to **50 gallery items total**, including **10 videos**.
- Each video must have a readable duration of **90 seconds or less** and a codec supported by the device.
- Select thumbnails, use previous/next, or swipe the main preview. Expand it for a larger view.
- Enable **Auto slideshow** and enter a positive duration in seconds to cycle through items.
- Videos play muted and inline, and pause when hidden or offscreen. They do not add their audio to your mix.
- To set a channel cover, select an image or GIF, choose a channel and press **Assign**. Removing the gallery item does not remove an already assigned cover.

Invalid imports report their reason. Valid items in the same batch can still be accepted. A video counts toward both the 50-item total and the 10-video limit.

## Five rotating backgrounds

The background manager holds **five images or GIFs**, each with its own positive display time. Choose a thumbnail, swipe, or use previous/next for manual selection. Edit each duration, then turn on **Auto cycle** to use those individual times.

At capacity, replace a selected background or remove one before adding another. Gallery slideshow timing and background timing are independent. The picture control in the top bar adjusts backdrop strength. The supplied wolf artwork provides the starting collection.

## Intent-led mini HUD and full player

The mini **Saved HUD** has a reserved dock below the routing canvas. Curves approach its top port, leaving the player clear of the network. Its port accepts connections in both directions; each route can be reversed or removed like any other link. Use **Open full Saved HUD** for the larger player.

With **Flow coupling on**, intent text leads the HUD's palette, pace, glow and breathing. Local keyword profiles include Calm / sleep, Focus / clarity, Grounded / safe, Energy / confidence, Release / growth and Love / connection. Unmatched text receives a repeatable **Custom text** appearance. These labels describe a local visual mapping, not an interpretation of your mind or a claim that the animation produces those outcomes. The readout shows which visual profile was selected. Routes, active audio and the flow settings add smaller visual accents.

The embedded player keeps the evolving effect visible instead of fading away after five seconds. **Play HUD / Pause HUD** controls its animation separately from audio playback. **Flow coupling off** restores the original style and pace while continuous visibility remains enabled. The mini view pauses when offscreen, the page is hidden or visual motion is paused. Mini and full views are separate animation instances; leaving the full screen closes that instance.

The full tab retains the Teal Apparitions player's controls, including **Captured moment**, **Restart from zero**, orbit, zoom, import/export and fullscreen. **Captured moment** restores the saved camera and timeline while continuous visibility remains enabled. In the phone apps, **Fullscreen** fills the app viewport and **Exit fullscreen** returns to the normal view. The browser preview also offers **Open original** for the untouched saved player. The separate Aether art layer has been removed.

### Capture a HUD image

1. Open **Saved HUD** and allow the artwork to finish loading. **Pause HUD** can hold a moment for capture.
2. Choose **Capture image**. The current HUD artwork is saved as a **PNG** in the app's local **Gallery** and counts toward its 50-item limit.
3. Choose **View captured image** to open Gallery. You can use the saved image like another gallery image, including assigning a channel cover or background through the normal media controls.
4. The browser preview additionally offers **Download PNG**. The native phone app saves into its own Gallery; it does not promise a separate Photos export.

If the player is still loading, frame access is unavailable or Gallery is busy/full, wait or free a Gallery slot and retry. Capturing an image does not record or change audio.

## Guide: playlists and optional recordings

Open the **Guide** tab for the two supplied playlists and five optional additional titles. **Open playlist** or **Find in playlist** opens YouTube or the phone's browser separately; return to Undertone when finished.

Expand a video's **Details / description** and check its **creator-pinned comments** for a free audio file **where the creator provides one**. Save that creator-provided MP3/WAV to Files or Downloads, then return to Studio and import it into a slot. A YouTube offline download stays inside YouTube and cannot be imported as a file. Use the creator's own download links and terms. A free-to-watch video does not establish that a downloadable file exists.

Keep the supplied five starters and use **slots 6–10** for optional additions. Direct watch URLs, uploader identity and free-file availability for those additional titles were not verified. Read [CREATOR-SOURCES.md](CREATOR-SOURCES.md) for the full titles, playlist verification and conditional instructions. Creator titles and field descriptions are not verified health or treatment benefits.

## Existing iPhone library

For an update of the older native iPhone app, keep the existing installation and sign the update with the same account and identity. The existing native library and mix are preserved. Open **Help (question-mark icon) → Native library** to browse saved recordings or make additional assignments, then choose **Return to Studio**; those changes update the studio when the native view closes. All ten studio slots use native audio for recordings and tones. The new visual network, gallery and backgrounds have their own local state. The installer does not transfer recordings from a different phone or desktop browser.

### Channel-cover storage and recovery

Channel pictures accept readable images up to **20 MB** and are stored separately from the mix settings. The mix keeps a reference to each picture; volume, position and seek changes do not rewrite its image bytes. Existing readable covers are migrated, and the older saved mix record is retained for recovery.

If an individual cover cannot be recovered, the app keeps its earlier record, shows fallback artwork and reports the channel in a warning. An unreadable cover is handled separately from the audio settings. Keep the installed app and original media while that warning is investigated; do not uninstall or clear storage to remove it.

The separate picture store concerns channel covers. Gallery, video, background and intent-image storage formats remain unchanged; the Gallery still holds 50 items including up to ten videos of 90 seconds or less. The larger portal vortex remains unchanged. See the release notes for the completed automated persistence checks and physical-device testing limits.

## Privacy and keeping your media

Imports and mix settings belong to this local app installation. There is no Undertone account or media-upload service. The shared starter recordings are part of the public installer; your later imports, mix and intent remain local. The operating system's own backup and file-provider behavior is separate.

Keep original files outside the app. Uninstalling, clearing app storage, signing as a different app identity or changing devices can remove or separate local data. Before updating, keep the current app installed and follow the platform guide. Do not treat an installer ZIP as a backup of your imported library.
