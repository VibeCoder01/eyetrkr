# Face-Tracked Wireframe Cube

A single-file HTML demo that renders a perspective wireframe cube and shifts
its depth based on your head position. It uses the device camera with native
FaceDetector when available and falls back to MediaPipe from a CDN.

## Quick Start

Because camera access requires `http://localhost` or HTTPS, run a local server:

```bash
python3 -m http.server
```

Then open `http://localhost:8000/index.html` and click **Enable camera**.
Fullscreen starts automatically after permission is granted.

## Project Structure

- `index.html` — app UI, styling, and face-tracked rendering (no build step).
- `AGENTS.md` — contributor guidelines.

## Notes & Requirements

- Best tested in Chrome or Edge.
- If native FaceDetector is unsupported, MediaPipe loads from
  `https://cdn.jsdelivr.net`.
- Camera data stays in the browser; nothing is uploaded.

## Troubleshooting

- If the demo is blank or clipped, refresh after entering fullscreen.
- If the camera fails, confirm you are on `localhost`/HTTPS and allow permissions.

## Customize

Edit `index.html` to tweak cube size, depth, or colors. The `drawCube` function
controls depth shifts and line/dot styling.
