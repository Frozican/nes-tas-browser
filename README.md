# NES TAS Browser v0.7

English-language browser NES TAS starter. Includes frame advance +/-1 and +/-10, jump to frame, vertical input timeline, hold/clear a controller button across a frame range, RAM watcher, TAS JSON import/export, savestate controls, and experimental frame-accurate MP4 export.

## Run
1. Extract the ZIP.
2. Open `index.html` in a recent browser with internet access (JSNES and the MP4 muxer load from CDNs).
3. Load your own `.nes` ROM.
4. Configure timeline inputs and use **Record from Frame 0 & Export MP4**. Set an exclusive end frame and output FPS.

## MP4 export notes
- Uses WebCodecs plus `mp4-muxer` loaded dynamically from a CDN. Browser support varies; if `VideoEncoder` is unavailable, MP4 export cannot run in that browser.
- It emulates and captures frames offline as quickly as encoding permits, applying the TAS input scheduled for each frame. It is not real-time capture.
- Audio is not included. Long recordings can use substantial memory because the MP4 is finalized in memory; test a short clip first on mobile.
- A practical end-frame limit of 30,000 is enforced, but mobile devices may handle much shorter clips depending on available memory.
- This build is not validated against every ROM, mapper, or mobile browser.

ROM files are processed locally in the page; they are not uploaded by this app.
