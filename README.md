# Computer-Vision-VAR-Offside-Visualisation
Goal: Analyse match video and overlay tracked players, pitch markings, and estimated offside positions.

Build plan
1. Use a pretrained object detector to identify players, referees, and the ball.
2. Track detections between frames using ByteTrack or a comparable tracker.
3. Detect pitch markings and estimate a camera-to-pitch homography.
4. Project player ground-contact points onto a 2D pitch.
5. Estimate the second-last defender's position at a manually selected pass frame.
6. Render offside reference lines and a top-down tactical view.
7. Test accuracy against manually annotated video frames.
Suggested stack: Python, OpenCV, YOLO, ByteTrack, PyTorch, React.

Module practice: Classification, evaluation, data preprocessing, cloud inference.

Evaluation: Detection precision/recall, tracking IDF1, pitch-coordinate error, and offside-line error.

Important scope: A student system should be presented as an experimental offside visualisation, not an official VAR replacement. Accurate offside decisions require precise timing, body-part localisation, camera calibration, and interpretation of the rules.

Extension: A browser interface with synchronised match footage, tactical camera view, and interactive overlays.
