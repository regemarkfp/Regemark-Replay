# Changelog

## 1.2.3 — 2026-11-14

**New**
- Hardware encoding: record the ISOs as H.264 or HEVC on the graphics card - NVIDIA NVENC, Intel Quick Sync (incl. the graphics built into Intel CPUs), AMD AMF, or VA-API on Linux. "Automatic" picks the first encoder that works; if none does, REC records SpeedHQ instead. About a third of SpeedHQ's size, CPU left free. Clip exports use the same encoder.
- Hardware decoding: H.264 / HEVC 4:2:0 files (hardware recordings, most ingested media) are decoded on the GPU (SETTINGS tick box, on by default). SpeedHQ stays on the CPU.

**Improved**
- Dropdowns instead of typing in SETTINGS: quick clip length, bitrate, handles, ATEM cut offset and input, HyperDeck port, DeckLink outputs (cards found on the PC), NDI sources and capture devices, audio trims, fast-jog frames, macro waits.

## 1.2.2 — 2026-11-14

**Improved**
- Much smoother reverse jog and shuttle far back from disk: every decoded picture is kept, several stretches further back are decoded in parallel before they are needed, and reverse starts at once from the pictures already decoded while playing forward. Rocking back and forth over the same moment is instant.
- A fast-spinning jog wheel scrubs like the shuttle at that speed, then settles on the exact frame when it stops.
- The time-to-OUT countdown (and PLAYLIST OUT) follows speed changes, also while paused or shuttling back.

## 1.2.1 — 2026-11-11

- Stable release of the 1.2 beta features below.
## 1.2.1 beta — 2026-11-07

**New**
- Screen outputs: any replay output - and the multiview / outputs view - clean and fullscreen on one of the PC's own screens (HDMI / DisplayPort used like a video output). No overlays, no frame, no mouse pointer.
- The version is shown in the top bar (`v1.2.1 beta`).

## 1.2.0 beta — 2026-11-03

**New**
- DeckLink output: each replay output on its own Blackmagic SDI / HDMI port, with embedded audio (2, 8 or 16 channels), locked to the card's clock.
- Monitoring feeds: the multiview and the outputs view rendered by the app and sent out over NDI and / or DeckLink.
- Tally lights on every camera and output window (red = program, green = preview), from NDI tally and the ATEM.
- ATEM auto-roll: an output plays its cued clip when the ATEM takes its input (cut or mix), like a HyperDeck.
- Guided tour on first start, and a TOUR button to replay it.

**Improved**
- The open project saves itself whenever shortcuts, X-keys, MIDI, macros or settings change, and when the app closes.

## 1.1.0 — 2026-11-03

**New**
- Source picker with live thumbnails for every camera input: NDI sources and DeckLink inputs found automatically.
- Timecode in recorded file names (`CAM1_21-52-18-08.mov`) and exported clips.
- ATEM → DaVinci Resolve: program cuts are logged while recording; export a Resolve timeline (FCP7 XML) and a multicam clip (FCPXML), optionally with DNx copies of the ISOs.
- Playlists: Mix / Dip / Wipe transitions per clip, PLAYLIST OUT countdown.
- FAST JOG (10 frames per jog click, shuttle up to 1000%) and SMOOTH slow motion.
- IN / OUT on any clip (ingested media too), with keys, buttons and "IN HERE / OUT HERE"; no limit to how far they move.
- Per-clip camera, Duplicate, clip edit bar.
- Clip stores: 4 pages × 10, STORE / CLEAR keys, store a specific camera, two-state button feedback (stored / on an output).
- Browse buttons for folders, shortcuts and projects; INGEST FOLDER.
- New look: dark grey (#262626) with RegemarkFP green (#00ff82), hard corners and slanted film-style buttons like the RegemarkFP logo.

**Linux (preview)**
- `.deb` package for Linux Mint 22 / Ubuntu 24.04: NDI, USB / HDMI capture cards, DeckLink (with a DeckLink-enabled ffmpeg), PulseAudio / PipeWire sound devices, X-keys and MIDI, app windows on every display, Install NDI helper.

**Improved**
- DeckLink inputs ask the card for the house video format (fall back to its default).
- Multiview / outputs view: clip names wrap instead of overlapping, larger countdown, shorter EVS-style meters.
- Installer: updates over a running or virus-scanned install, shows the real error if it can't.

## 1.0.2 — 2026-11-02

First public release: up to 8 cameras (NDI / DeckLink), SpeedHQ ISO recording, EVS-style replay from live with jog / shuttle (memory buffer), up to 8 outputs, clips, media ingest, playlists, multiview, X-keys / MIDI / keyboard control, ASIO / Dante audio, projects.
