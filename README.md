# Pocket Pads

A deliberately simple, phone-first sampler (a "Koala-lite"). No install, no build, one file.

**Three tabs, one record button**
- **Pads** – 16 pads. Tap to play. Tap an empty pad, hit **● Record**, hit **Stop**: it's trimmed, normalised and saved on that pad.
- **Keys** – the selected pad's sound, pitched across a 2-octave piano keyboard (Oct −/+ to shift).
- **Beat** – 16-step drum machine with tempo slider; every pad that has a sound gets a row. Your recordings are drum sounds too.

Comes with 8 built-in synthesised drum sounds, so it makes noise immediately.
Recordings are stored on-device (IndexedDB); beat + tempo in localStorage.

## Run
`python3 -m http.server` then open `http://<your-ip>:8000` on the phone. Microphone access requires **https or localhost**
(host it on GitHub Pages / Netlify for real phone use, then "Add to Home Screen").

## Roadmap ideas
Sample trimming, pad-recording straight from the beat, per-step velocity, loop-record multi-track, export WAV, share link, PWA offline manifest.
