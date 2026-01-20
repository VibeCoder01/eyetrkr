# Face-Tracked Wireframe Cube

A single-file HTML demo that renders a perspective wireframe cube and shifts
its depth based on your head position. It uses the device camera with native
FaceDetector when available and falls back to MediaPipe from a CDN.
<img width="1133" height="563" alt="image" src="https://github.com/user-attachments/assets/bff98a04-d3b5-4690-b0fc-cfcc630d4e7d" />
<img width="759" height="721" alt="image" src="https://github.com/user-attachments/assets/82a62d3b-dda6-440d-a65d-2f6435aab20a" />

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
