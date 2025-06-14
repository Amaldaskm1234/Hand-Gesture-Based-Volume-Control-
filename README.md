# Hand-Gesture-Based-Volume-Control-
This AI-based computer vision system controls system volume using hand gestures. By tracking the distance between thumb and index finger via webcam, it adjusts the volume in real time, offering a touch-free, intuitive alternative to physical controls.
Project Description: Hand Gesture-Based Volume Control System
This project is an AI-powered computer vision application that allows users to control their computer's system volume using simple hand gestures. By leveraging a webcam and real-time hand tracking, it eliminates the need for physical touch, making it highly intuitive and touchless.

The system captures live video through a webcam and uses a hand tracking module (built on top of MediaPipe) to detect and track the position of the user's hand. Specifically, it monitors the tips of the thumb and index finger. When the user brings these two fingers closer together or farther apart, the system measures the distance between them using basic geometry (Euclidean distance).

This distance is then mapped to the system’s volume range using interpolation. For example, a small distance might set the volume to 0%, while a wider spread between fingers sets it to 100%. This change is applied to the Windows master volume in real time using the pycaw (Python Core Audio Windows) library.

In addition to gesture detection and volume control, the program provides real-time visual feedback. This includes drawing circles on the fingertips, a line connecting them, a volume level bar, percentage display, and frames-per-second (FPS) information—all overlaid on the video stream using OpenCV.

The solution is ideal for situations where hands-free interaction is beneficial—like during presentations, in clean environments, or for users with physical limitations. It serves as an innovative example of combining computer vision, gesture recognition, and system-level integration.
