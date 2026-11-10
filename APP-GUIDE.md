# Use Undertone Studio

The expanded studio combines ten audio slots with a visual network and a private media collection. The flow diagram and intent text are visual organization tools. They do not route audio signals, change a recording's contents or establish a subliminal, medical or therapeutic effect.

## First listen

1. Lower your phone's output volume, open Undertone and allow the interface to finish loading.
2. Select **Import audio** or an empty channel, then choose an MP3 or WAV. If it is stored in a cloud file provider, download the file before importing.
3. Tap Play for that channel. **Pause** keeps its position; **Stop** rewinds. Use the bottom transport to control the mix. Saved audio returns paused on a new launch.
4. Add more recordings, up to **ten slots**. A slot can hold a recording, a generated tone or both. Importing into an occupied slot replaces that slot's recording.
5. Tap a channel name or its controls button to adjust level, seek, mute, looping and stereo position. Optional automatic panning moves between its selected bounds.
6. Test the app with the phone locked and with your usual second media app before relying on a long background session. Calls, alarms, device controls and other apps can interrupt playback. Use the platform installation guide if background playback stops.

On a narrow screen, **Flow**, **Channels** and **Media** switch workspaces. The bottom master transport remains available.

On Android, the native media notification also provides Play/Pause/Stop. Headphone disconnection and phone/communication mode pause playback. Long imports decode to disk and can use about 1.4 GB per hour; see the [Android storage limits](ANDROID-INSTALL.md) before importing a large collection. The iPhone version also uses native audio; the visual interface is not responsible for keeping audio running while the phone sleeps.

## Master level and generated tones

The master runs from **0% to 1,100%**. At 100% it adds no master boost; 1,100% represents 11 times nominal digital amplitude before output limiting. It cannot make the phone's amplifier 11 times stronger, and an already-loud recording may gain little extra loudness because the limiter contains peaks. Set comfortable device volume first, then adjust the mix gradually.

Each slot's optional tone has its own level, stereo controls and carrier frequency up to **20,000 Hz**. Carrier choices are sine, triangle, square, sawtooth, pulse, asymmetric, parabolic, sinc and fractal. Modulation changes the carrier's amplitude; it is separate from carrier frequency. Very high settings may be inaudible or limited by the phone and output device. No audible tone is not a reason to raise the output abruptly.

## Create and edit the visual network

The network has **12 endpoints**: **Core**, channels **1–10**, and **HUD**. Empty channels can participate; adding or clearing a recording does not delete their visual routes.

1. Tap **Set intent** to enter text and choose a color.
2. Turn on **Link mode**, choose an origin port, then choose one or more destinations. The origin remains selected for branching. You can also drag between ports, including from the Core's connection button or port.
3. Core, channels and HUD can each be either origin or destination. **Both directions** in the connection dialog creates two directional links.
4. Tap a curve to edit it, reverse its direction or remove it. A reverse changes the visual link, not audio playback. When the reverse direction already exists, reversing merges into that existing direction instead of creating a duplicate.
5. Drag channel title bars to arrange the cards. Resetting layout leaves your links intact.
6. Use **Apply to visualization** to keep dialog changes, or **Cancel** to discard them. Canvas edits begin saving after each change.

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

## Mini HUD and the full preserved player

The mini **Saved HUD** has its own reserved dock below the routing canvas, inside the Flow panel. Curves approach its top port, leaving the player clear of the network. Its port accepts connections in both directions, and each connection can be reversed or removed just like any other link.

Use its **Pause/Resume** control or **Open full Saved HUD**. The full tab exposes the preserved Teal Apparitions player's original controls, including **Captured moment**, **Restart from zero**, orbit, zoom, import/export and fullscreen. In the phone apps, **Fullscreen** fills the app viewport and **Exit fullscreen** returns to the normal view. **Open original** is available only in the browser version. Mini and full views use separate playback instances.

Both load the same preserved player HTML. The mini wrapper crops the original stage; it does not replace the effect or rewrite its source. The miniature pauses effect time when offscreen, on a hidden page, or when visual motion is paused.

## Existing iPhone library

For an update of the older native iPhone app, keep the existing installation and sign the update with the same account and identity. The existing native library and mix are preserved. Open **Help (question-mark icon) → Native library** to browse saved recordings or make additional assignments, then choose **Return to Studio**; those changes update the studio when the native view closes. All ten studio slots use native audio for recordings and tones. The new visual network, gallery and backgrounds have their own local state. The installer does not transfer recordings from a different phone or desktop browser.

## Privacy and keeping your media

Imports and mix settings belong to this local app installation. There is no Undertone account or media-upload service. The shared starter recordings are part of the public installer; your later imports, mix and intent remain local. The operating system's own backup and file-provider behavior is separate.

Keep original files outside the app. Uninstalling, clearing app storage, signing as a different app identity or changing devices can remove or separate local data. Before updating, keep the current app installed and follow the platform guide. Do not treat an installer ZIP as a backup of your imported library.
