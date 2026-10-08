# Insomnia OS 🌙

A cozy retro desktop for 4 AM. Boot it up, mix a sleep soundscape, count some sheep, jot down what's keeping you awake, watch the stars, then shut down gently.

**Live:** https://insomnia-os.sites.tab.bot/

## What's inside
- 🌧️ **Soundscape.exe**: rain, fan hum, old computer whir (with hard-drive chatter) and crickets, all synthesized live with the Web Audio API. No audio files. Each channel has its own labelled volume slider, plus presets.
- 🐑 **Sheep.exe**: a sheep counter with a synthesized "baa", milestones, and a count that persists.
- 📝 **4am Thoughts.txt**: a local-first notepad. Saved to `localStorage`, never leaves your device. Export as .txt.
- ✨ **Starfield.scr**: classic warp starfield; static under reduced motion. Any key or tap wakes it.
- 🛌 **Shut Down**: a gentle chime, an optional "keep the soundscape playing", and "Goodnight 🌙".
- 🔊 Classic synthesized UI sounds with a global mute (remembered).

## Accessibility
- Every window is a labelled, non-modal `role="dialog"`; focus moves into a window when it opens and back to its icon when it closes. Escape closes.
- Desktop icons are a toolbar with roving focus (arrow keys, Home/End, Enter).
- Windows move by mouse/touch drag or by keyboard (the ⠿ grip button + arrow keys, Shift for bigger steps).
- Taskbar lists open windows (`aria-current` on the active one).
- Sliders have visible labels, live percentage outputs and `aria-valuetext`.
- Polite live-region announcements for state changes; skip link; strong visible focus; high-contrast palette; `forced-colors` support.
- `prefers-reduced-motion` honoured (no boot animation, no hopping sheep, static stars).
- No sound plays before your first press.

## Run locally
It's plain HTML, CSS and JavaScript, so no build step is needed. Open `index.html`, or serve the folder:

```
python3 -m http.server 8000
```

## Credits
Idea and inspiration: **Hasan ([2three1y](https://2three1y.github.io/))**, who couldn't sleep.
Made by Tab for Hasan at 4 AM.

## License
MIT. See [LICENSE](LICENSE).
