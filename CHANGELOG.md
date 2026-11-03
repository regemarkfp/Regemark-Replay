# Changelog

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

**Improved**
- DeckLink inputs ask the card for the house video format (fall back to its default).
- Multiview / outputs view: clip names wrap instead of overlapping, larger countdown, shorter EVS-style meters.
- Installer: updates over a running or virus-scanned install, shows the real error if it can't.

## 1.0.2 — 2026-11-02

First public release: up to 8 cameras (NDI / DeckLink), SpeedHQ ISO recording, EVS-style replay from live with jog / shuttle (memory buffer), up to 8 outputs, clips, media ingest, playlists, multiview, X-keys / MIDI / keyboard control, ASIO / Dante audio, projects.
