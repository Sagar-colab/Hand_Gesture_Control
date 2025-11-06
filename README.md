Hand HUD — palm-anchored kinematic dashboard

By-Sagar.U

This project captures webcam input, detects a hand using MediaPipe, and draws a white, mechanical-style kinematic HUD over the hand (palm-centered radial UI, finger bones, rotation readout, small 3D cube and grid) similar to the reference images.

## Files

- `requirements.txt` — Python dependencies
- `main.py` — application entrypoint and webcam loop
- `hand_overlay.py` — functions for drawing the HUD and computing kinematics
- `utils.py` — small helpers (smoothing, geometry)

## How to run (Windows PowerShell)

1. Create and activate a virtual environment (optional but recommended):

   python -m venv .venv; .\.venv\Scripts\Activate.ps1

2. Install dependencies:

   pip install -r requirements.txt

3. Run:

   python main.py

## Notes

- Works with a single hand in frame. For multi-hand, toggle a flag in `main.py`.
- Tweak smoothing and drawing constants in `hand_overlay.py`.
- If you want recording/output images, I can add that next.



