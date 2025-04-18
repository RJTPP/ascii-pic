# ASCII File Import & Preview

A self-contained HTML application that lets you import an image or video file, configure ASCII rendering parameters, preview the output in real time, and save snapshots or recordings — all entirely in the browser with no external dependencies.

## Features

- **File Import**
  - Single `<input type="file">` accepts both images and videos.
  - Automatically detects file type and switches into **Image Mode** or **Video Mode**.

- **ASCII Preview**
  - Renders into a `<pre>` element using a monospaced font.
  - Uses an off-screen `<canvas>` to sample pixels, compute luminance → ASCII characters, and (optional) glyph colorization.
  - Preserves proper aspect ratio using a character-aspect correction factor.

- **Save Functionality**
  - **Image Mode** → Exports a single PNG snapshot of the ASCII canvas.
  - **Video Mode** → Records ASCII frames into an WebM and downloads the file.

## Usage

1. **Load the HTML**
   - Open `index.html` in any modern browser (Chrome, Firefox, Safari, Edge).

2. **Import a File**
   - Click **File** and select an image (PNG, JPG, etc.) or a video (MP4, WebM).

3. **Configure**
   - Adjust **Width** (columns), **Contrast**, and toggle **Color**.
   - In **Image Mode**, the preview updates instantly.
   - In **Video Mode**, press **Play** to start rendering; press **Pause** to tweak settings.

4. **Save**
   - Click **Save** to download:
     - A **PNG** snapshot for images.
     - An **MP4** (or WebM) video for recordings.
   - Watch the progress bar for feedback during the export.


## License

This project is released under the [MIT License](LICENSE).

You are free to use, modify, and distribute this software under the terms of the MIT License. See the LICENSE file for detailed terms and conditions.


