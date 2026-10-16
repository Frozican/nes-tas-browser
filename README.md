# 🎮 NES TAS Browser

**A browser-based NES emulator and Tool-Assisted Speedrun (TAS) editor.**

Play NES games, edit controller inputs frame by frame, build precise TAS sequences, inspect memory, and experiment with high-speed gameplay recording — all through a web interface.

<p align="center">
  <a href="https://frozican.github.io/nes-tas-browser/"><strong>🚀 Play NES TAS Browser</strong></a>
</p>

> **Current version: v0.7 — Experimental**
>
> Some features, especially MP4 export, may have browser-specific limitations and have not been tested across all devices.

## ✨ Features

- 🕹️ **NES Emulation** — Load your own `.nes` ROM files.
- 🎯 **Frame-Perfect Editing** — Create and edit controller inputs frame by frame.
- ⏩ **Frame Advance** — Move forward or backward by 1 or 10 frames.
- 🔢 **Jump to Frame** — Navigate directly to a specific frame.
- 🎹 **Vertical TAS Timeline** — Edit inputs in a piano-roll-style interface.
- 🔁 **Range Input Editing** — Hold a selected controller button over a chosen frame range.
- ▶️ **Playback Controls** — Play, pause, step through frames, and reset gameplay.
- 💾 **Save States** — Save and restore emulator state where supported.
- 🧠 **RAM Watcher** — Monitor selected NES memory addresses.
- 🎥 **Experimental Recording** — Process gameplay from frame 0 and attempt MP4 export.
- 📱 **Mobile-Friendly UI** — Designed for desktop and mobile browsers.
- 🌐 **Browser-Based** — No traditional desktop installation required.

## 🚀 Getting Started

### Play online

Open the live website:

**[https://frozican.github.io/nes-tas-browser/](https://frozican.github.io/nes-tas-browser/)**

1. Open the website in a modern browser.
2. Select **Load NES ROM**.
3. Choose a `.nes` ROM file from your device.
4. Start playing or create a TAS using the timeline and frame controls.

The website does not provide copyrighted game ROMs. You must supply your own ROM files.

### Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Load a compatible `.nes` ROM file.

Depending on the browser and the features being used, opening the file directly may not work for every function. If necessary, serve the files through a local web server.

## 🎮 TAS Controls

| Control | Function |
|---|---|
| Frame −1 / +1 | Step one frame backward or forward |
| Frame −10 / +10 | Step ten frames backward or forward |
| Jump to Frame | Navigate to a specific frame |
| Play / Pause | Control emulation playback |
| Reset | Reset the emulated game |
| Range Input | Hold a selected button across a frame range |
| Clear Range | Remove inputs from a selected range |
| Save State | Save the current emulator state, where supported |
| Load State | Restore a saved emulator state, where supported |
| RAM Watcher | Inspect selected memory addresses |
| Record / Export | Experiment with frame-based recording and MP4 export |

The exact controls and availability depend on the current application version.

## 🎥 Recording and MP4 Export

The experimental recording feature is designed to:

1. Start emulation from frame 0.
2. Process gameplay frames without waiting for real-time playback.
3. Capture the rendered frames.
4. Encode the captured frames into an MP4 video, where supported.

### Current limitations

- Browser and encoder compatibility may vary.
- Long recordings can consume substantial memory.
- Audio recording is not currently supported.
- Recording performance depends on the device and the emulation workload.
- MP4 export has not been verified across all browsers and devices.

**Recommendation:** Start with a short recording before attempting a long TAS.

## 🧠 ROM Compatibility

The emulator uses JSNES for NES emulation. Compatibility depends on the emulator core, supported mapper hardware, ROM format, and browser environment.

Some games may not work correctly, especially those that require specialized cartridge hardware or mapper support.

If a game fails to load, please report the game, ROM region, browser, and any error message. Do not upload copyrighted ROM files to an issue.

## 🔒 Privacy

ROM files are selected by the user through the browser interface and are intended to be loaded locally.

The application may load external JavaScript libraries or encoding resources, depending on the implementation. Therefore, do not assume that every feature works completely offline.

Never upload ROM files or other copyrighted material to the repository without the necessary rights.

## 🛠️ Technology

- HTML
- CSS
- JavaScript
- [JSNES](https://github.com/bfirsh/jsnes)
- Browser APIs for rendering, input, and media processing

See the respective dependency repositories for their source code and license terms.

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome!

When reporting a bug, please include:

- Browser and version
- Operating system and device
- Game title and ROM region
- Steps to reproduce the issue
- Expected and actual behavior
- Screenshots or error messages, if available

Please do not attach copyrighted ROM files.

## 🗺️ Roadmap

Potential improvements include:

- [ ] Improve compatibility with more NES mapper types.
- [ ] Improve color accuracy and rendering consistency.
- [ ] Make TAS playback and input recording more reliable.
- [ ] Improve RAM inspection and debugging tools.
- [ ] Improve recording performance and browser compatibility.
- [ ] Expand automated testing across browsers and devices.

## 📄 License

This project is licensed under the **MIT License**. See the [`LICENSE`](LICENSE) file for details.

Third-party dependencies remain subject to their own license terms.

## 🙌 Acknowledgements

- [JSNES](https://github.com/bfirsh/jsnes) for NES emulation.
- The open-source emulator and TAS communities for their work and inspiration.

---

**Built for frame-by-frame precision. Made for the TAS community.**

⭐ If you find this project useful, consider starring the repository!
