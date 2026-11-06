# MotionSync Coach

**MotionSync Coach** is a mobile application built with Flutter that uses TensorFlow's MoveNet model for pose detection to help users count reps and detect the correctness of their form. Train anywhere, anytime with just a camera-enabled device. The app includes BMI calculation, nutrition tracking, and user authentication via Firebase.

## Expected Outcomes

The app is designed to deliver:

- **Enhanced User Engagement** — The interactive platform makes exercise sessions more engaging and motivating, encouraging users to continue their fitness journey.
- **Accessibility and Convenience** — Users can train anywhere and anytime with just a camera-enabled device, making personal training accessible.
- **Promotion of Safe Exercise Habits** — By guiding users toward proper exercise techniques, the system aims to reduce the risk of injuries and improve workout efficiency.
- **Educational Video Support** — When an incorrect movement is detected, the system automatically displays a short educational video that explains and demonstrates the proper technique (in-app GIF + optional YouTube tutorial).
- **Real-time Feedback** — Users receive immediate on-screen feedback indicating whether their form is correct or not, helping them correct mistakes instantly.

## Features

- **Reps counter** — MoveNet-based pose detection to count reps for each exercise.
- **Pose correctness detection** — Custom ML models (TFLite) on MoveNet keypoints to classify form and provide correction advice.
- **Real-time form feedback** — Live form score bar, instant CORRECT / ADJUST FORM badge, and spoken guidance.
- **Educational correction popups** — When form is wrong, a short tutorial (GIF + message + “Watch tutorial video” for YouTube) appears to demonstrate proper technique.
- **Voice control** — Hands-free commands on the camera screen (e.g. start warmup, start workout, complete set).
- **Progress reports** — Accuracy percentage, most common mistakes, and improvement over time (viewable in-app and stored in Firestore).
- **Settings** — Camera permissions, feedback language (e.g. English, Arabic, Spanish), and exercise difficulty presets.
- **BMI calculator**, **nutrition tracker**, and **Firebase authentication**.

## Technologies Used

- **Flutter** — Cross-platform UI (Android, iOS, web, desktop).
- **TensorFlow Lite** — MoveNet for pose estimation; custom form classifiers per exercise.
- **Firebase** — Auth and Firestore for profiles, workout history, and progress data.

## Getting Started

1. Clone the repository and open the project.
2. Install dependencies:

   ```bash
   flutter pub get
   ```

3. Run the app:

   ```bash
   flutter run
   ```

Ensure Android NDK is installed (e.g. 27.x or as required by your Flutter/plugin setup) and that camera (and optionally microphone for voice) permissions are granted.

## Contributing

1. Fork the repo and create a branch for your feature or fix.
2. Follow the project’s coding standards and test your changes.
3. Submit a pull request with a clear description of your changes.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
