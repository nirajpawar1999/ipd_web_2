# IPD (Browser) — On-device Interpupillary Distance Estimator

This is a browser app that measures IPD using the front camera.  
All processing runs on the device. No video or data leaves the browser.

- MediaPipe Face Landmarker (web) for 478 landmarks (incl. iris).
- f_px calibration at ~30 cm.
- Optional personal iris size calibration.
- Robust smoothing (median + MAD).
- Shows IPD in pixels and centimeters.
- Adds a fixed **+0.6 cm** to the computed IPD to match your field tests.

---

## Live demo

- GitHub Pages: **`https://<your-username>.github.io/<your-repo>/`**

> Works on mobile and desktop. Use HTTPS. iOS Safari needs user interaction to start the camera.

---

## Quick start

Clone and open with a static server:

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

# Option A (Node)
npx serve

# Option B (Python 3)
python -m http.server 8080
