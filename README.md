# NES TAS Browser

A browser-based NES emulator and Tool-Assisted Speedrun (TAS) editor. Play NES games, edit controller inputs frame by frame, and experiment with deterministic playback and video export — right in your browser.

> **Status: Experimental — v0.7**
>
> Features and browser compatibility are still being tested. Video export may depend on browser support and external resources.

## ✨ Features

- **NES emulation** — Load your own `.nes` ROM files locally.
- **Frame-by-frame control** — Advance or rewind one frame at a time.
- **Fast frame advance** — Move forward or backward by 10 frames.
- **Jump to frame** — Navigate directly to a specific frame number.
- **TAS input timeline** — Edit controller inputs for individual frames.
- **Range input editing** — Hold a selected button across a chosen frame range.
- **Playback controls** — Play, pause, and reset gameplay.
- **Save states** — Save and restore emulator state where supported.
- **RAM Watcher** — Inspect selected memory addresses during gameplay.
- **Recording and video export (experimental)** — Process gameplay from frame 0 and attempt to export it as an MP4.
- **Mobile-friendly interface** — Designed to be usable on desktop and mobile browsers.

## 🚀 Getting Started

### Option 1: Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Load a `.nes` ROM file using the ROM upload control.
4. Use the playback controls and TAS timeline to play and edit inputs.

Some features may require a local web server or additional browser capabilities, depending on your browser and configuration.

### Option 2: Host with GitHub Pages

1. Push the project files to a public GitHub repository.
2. Open the repository's **Settings**.
3. Navigate to **Pages**.
4. Select the branch and folder containing `index.html`.
5. Save and open the published URL.

If the project uses external libraries or encoders, those resources must also be accessible for the corresponding features to work.

## 🎮 TAS Controls

| Feature | Description |
|---|---|
| Frame −1 / +1 | Move by one frame |
| Frame −10 / +10 | Move by ten frames |
| Jump to Frame | Navigate to a specified frame |
| Play / Pause | Control emulation playback |
| Reset | Restart the emulated game |
| Range Input | Apply a button hold over a frame range |
| RAM Watcher | Monitor selected memory addresses |
| Record / Export | Experiment with frame-based recording and MP4 export |

Exact behavior may vary by version and browser. Refer to the controls displayed in the application.

## 🎥 Recording and Export

The experimental recording feature is intended to process gameplay from frame 0, capture frames without relying on real-time playback speed, and export a video.

**Limitations:**
- MP4 encoding depends on browser support and the encoder implementation.
- Long recordings may consume substantial memory.
- Audio recording is not currently supported.
- Recording speed and compatibility have not been verified across all browsers and devices.

Test with a short recording before attempting a long session.

## 🧠 ROM Files and Copyright

This project does not include commercial game ROMs.

Load only ROM files you are legally permitted to use. Do not upload copyrighted ROMs to the repository unless you have the necessary rights.

ROM files selected through the browser are intended to be loaded locally by the application.

## 🛠️ Technology

- HTML, CSS, and JavaScript
- JSNES for NES emulation
- Browser APIs for rendering and input handling
- Experimental browser-based video encoding

See the relevant dependency documentation and license files for details.

## ⚠️ Known Limitations

- The project is experimental and may contain bugs.
- Video export and save-state behavior require further testing.
- Emulator color rendering may need additional fixes.
- Browser compatibility can vary, particularly on mobile devices.
- TAS timing and playback accuracy should be validated before relying on recordings for speedrun verification.

## 🤝 Contributing

Bug reports, feature requests, and contributions are welcome.

When reporting a bug, include:
- Browser and operating system
- Device type
- Steps to reproduce the issue
- Expected and actual behavior
- Screenshots or console errors, if available

## 📄 License

Choose and add a license before distributing the project. The license must be compatible with the project's dependencies and their terms.

If you choose the MIT License, include the corresponding `LICENSE` file and copyright notice.

## 🙌 Acknowledgements

- [JSNES](https://github.com/bfirsh/jsnes) — NES emulation library
- The open-source emulator and TAS communities

---

**NES TAS Browser** — Frame by frame, input by input.
