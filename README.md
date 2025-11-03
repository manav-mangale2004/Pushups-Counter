🏋️‍♂️ AI-Powered Push-Up Counter (Real-Time Pose Detection)

This project uses AI-based pose estimation and computer vision to automatically count push-ups in real-time through a standard webcam. By tracking shoulder, elbow, and wrist landmarks, the system accurately detects the user’s position, evaluates rep quality, and provides visual feedback — no sensors required!

✅ Features

🎯 Real-time pose tracking using MediaPipe

🔢 Automatic push-up rep counting

📐 Angle-based form detection (shoulder-elbow-wrist)

🚦 “Up” and “Down” state classification

🧠 Minimum hold-time filtering (reduces jitter false-positives)

🎥 Smooth UI overlay with FPS counter

🤖 Form correction hints (body alignment, depth cues)

🔁 Reset counter shortcut (press R)

❓ Toggle help prompt (press H)

🧠 How It Works

The system:

Processes webcam frames using MediaPipe Pose

Detects 3D body landmarks (x, y, confidence)

Calculates elbow joint angles

Classifies movement into states:

UP (arm extended ~160°+)

DOWN (arm bent ~70°–90°)

Increments the counter only on valid DOWN → UP transitions

Applies visibility confidence filters to avoid ghost reps
