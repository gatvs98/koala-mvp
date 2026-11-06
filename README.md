# Pocket Pads

A deliberately simple, phone-first sampler (a "Koala-lite"). No install, no build, one file.

**Three tabs, one record button**
- **Pads** – 16 pads. Tap to play. Tap an empty pad, hit **● Record**, hit **Stop**: it's trimmed, normalised and saved on that pad.
- **Keys** – the selected pad's sound, pitched across a 2-octave piano keyboard (Oct −/+ to shift).
- **Beat** – 16-step drum machine with tempo slider; every pad that has a sound gets a row. Your recordings are drum sounds too.

**Record hits live:** on the Beat tab press **● Rec hits** and tap the pads under the grid while the loop plays. Each tap snaps to the nearest step. **↶ Undo** removes the last take.

**Rename and erase:** tap the pad name in the bottom bar (✎) to rename it. Erase removes a sound for good, built-in drums included.

**Mix:** on the Beat tab, **🎚 Mix** opens a master volume and one slider per sound (0–150%). It applies to pads, keys, the beat and the export, and is saved.

**Export:** on the Beat tab pick 1–8 loops and press **⬇ Export WAV**. On phones it opens the share sheet (Save to Files, AirDrop, messaging apps); on desktop it downloads.

Installable as a PWA (home-screen icon, fullscreen, works offline once loaded). If you change a cached file, bump `VERSION` in `sw.js`.

Comes with 8 built-in synthesised drum sounds, so it makes noise immediately.
Recordings are stored on-device (IndexedDB); beat + tempo in localStorage.

## Run
`python3 -m http.server` then open `http://<your-ip>:8000` on the phone. Microphone access requires **https or localhost**
(host it on GitHub Pages / Netlify for real phone use, then "Add to Home Screen").

## Roadmap ideas
Sample trimming, chop mode, per-step velocity, loop-record multi-track, export WAV, share link, PWA offline manifest.
