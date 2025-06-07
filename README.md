# Gym-Pose-Estimation-Repetition-Counter

The goal of this project is to create a lightweight pose estimation system that takes a video stream (live or recorded) of a person performing exercises (e.g., pushups, squats, dumbbell curls), detects body landmarks, analyzes, and counts the number of completed repetitions per exercise.

---

This tool is designed to support home workouts, gym form correction, and personal fitness tracking using accessible hardware, such as Raspberry Pi or other Linux-based computers equipped with a USB camera.

## Workflow for Project

### Input: A live video stream or a recorded video

- Hardware: USB Camera
- A small resource-constrained computing platform like Raspberry Pi/Some other Linux SBC

### Software Tools

- Python 
- OpenCV
- PyTorch / Tensorflow Lite
- MediaPipe

### Tasks and Computing

- Input: Logging video / Stream
- JSON-based config support for multiple exercise definitions
- Pose detection (Key body landmarks)
- Angle calculation
- State Machine Logic (For Tracking exercises)

### Output

- Overlayed Video with Pose Skeleton
- Exercise Label
- Current angle between joints
- Rep count for the exercise
- Stored timestamped rep counts & form accuracy for post analytics
- Export of each session data as CSV/JSON file

### Future Work

- Inference on Jetson Nano, Google Coral TPU, Pi AI Hat, or some other AI accelerator board
- Real-time feedback
