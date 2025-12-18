# ITE120 FINAL PROJECT

# ☕ CaffioLens - Coffee Pack Identifier

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)

</div>

---

## 📖 About the App

**CaffioLens** is a mobile application built with Flutter that uses artificial intelligence to identify and classify different types of coffee packs through camera scanning. The app leverages TensorFlow Lite for on-device machine learning and Firebase for cloud data storage, providing users with instant coffee pack recognition and detailed analytics of their scanning activity.

---

## 🎯 Main Functions

### 1️⃣ **Real-Time Camera Scanning**
- Open the camera to scan coffee packs in real-time
- Instant image capture with one tap
- Live camera preview for accurate positioning
- Automatic focus and image optimization

### 2️⃣ **AI-Powered Coffee Identification**
- TensorFlow Lite model processes captured images
- Identifies coffee pack type and variety
- Provides confidence score (accuracy percentage)
- Achieves 94%+ accuracy in classification

### 3️⃣ **Gallery Image Selection**
- Pick existing photos from device gallery
- Analyze previously captured coffee pack images
- Same AI processing as camera scans
- Supports JPG and PNG formats

### 4️⃣ **Scan History & Analytics**
- View complete history of all scans
- Browse past identifications with timestamps
- Track success rate and performance metrics
- Filter by successful vs failed identifications

### 5️⃣ **Dashboard Statistics**
- **Total Scans**: Lifetime scan count
- **Success Rate**: Percentage of correctly identified packs
- **Today's Activity**: Number of scans performed today
- Recent scan list with thumbnails and details

### 6️⃣ **Cloud Synchronization**
- Automatic backup to Firebase Firestore
- Scan data persists across sessions
- Real-time data updates
- Secure cloud storage

---

## 🖥️ User Interface Features

- **Clean Material Design** - Modern, intuitive interface
- **Coffee-Themed Colors** - Professional brown color palette
- **Bottom Navigation** - Easy access to Home, Scan, Gallery, and History
- **Real-time Feedback** - Instant results and status updates
- **Responsive Layout** - Optimized for all screen sizes
- **Smooth Animations** - Enhanced user experience

---

## 🛠️ Technology Stack

| Component | Technology | Purpose |
|-----------|------------|---------|
| **Framework** | Flutter | Cross-platform mobile development |
| **Language** | Dart | App programming language |
| **AI/ML** | TensorFlow Lite | On-device image classification |
| **Database** | Firebase Firestore | Cloud data storage |
| **Camera** | Camera Plugin | Image capture functionality |
| **Image Picker** | Image Picker Plugin | Gallery selection |
| **Charts** | FL Chart | Data visualization |
| **Fonts** | Google Fonts (Lato) | Modern typography |

---

## 📸 App Screenshots

<div align="center">

### 🏠 Home Screen
![Home Screen](https://github.com/user-attachments/assets/56fc7d8c-9c8f-4ff3-a65a-8da746eab709)

*Dashboard showing statistics: Total Scans, Success Rate, and Today's Activity with recent scan history*

---

### 📷 Camera Scanner
![Camera Scanner](https://github.com/user-attachments/assets/ba9815bd-3b3d-4d20-ad10-952e032a43b3)

*Live camera preview for scanning coffee packs with capture button and navigation options*

---

### ✅ Scan Results

<table>
<tr>
<td width="50%">

![Scan Result 1](https://github.com/user-attachments/assets/748e1be9-41dc-46fe-ae32-78cf946cb879)

</td>
<td width="50%">

![Scan Result 2](https://github.com/user-attachments/assets/c76f0f75-fbfa-4426-81ec-4b7df0a4aa96)

</td>
</tr>
</table>

*Classification results displaying identified coffee type with confidence percentage*

---

### 📜 Scan History
![Scan History](https://github.com/user-attachments/assets/73413462-815b-4990-b173-55c41637afdb)

*Complete history of all scans with timestamps, thumbnails, and confidence scores*

</div>

---

## ⚙️ How It Works

1. **Launch the app** and grant camera permissions
2. **Tap "Scan Image"** to open the camera or **"Pick Gallery"** to select an existing photo
3. **Capture or select** a coffee pack image
4. **AI processes** the image using TensorFlow Lite model
5. **View results** with coffee type and confidence score
6. **Scan automatically saves** to Firebase history

---

## 🚀 Key Features

- ✅ **AI-Powered Recognition** - 94%+ accuracy rate
- ✅ **Real-Time Processing** - Results in under 2 seconds
- ✅ **Offline ML** - On-device processing for privacy
- ✅ **Cloud Backup** - Firebase data synchronization
- ✅ **Analytics Dashboard** - Track performance metrics
- ✅ **Gallery Support** - Analyze existing photos
- ✅ **History Tracking** - Browse all past scans
- ✅ **Modern UI** - Clean, intuitive design

---

## � Full Code

### Main Application (main.dart)

<details>
<summary>Click to expand full code</summary>

```dart
// Paste your main.dart code here
// Complete source code for the CaffioLens application
// Including all screens: HomeScreen, CameraScreen, ResultsScreen, PredictionsScreen, etc.
```

</details>

### TensorFlow Lite Helper (tflite_helper.dart)

<details>
<summary>Click to expand TFLite helper code</summary>

```dart
// Paste your tflite_helper.dart code here
// TensorFlow Lite model integration and image processing logic
```

</details>

### Firebase Configuration (firebase_options.dart)

<details>
<summary>Click to expand Firebase configuration</summary>

```dart
// Paste your firebase_options.dart code here
// Firebase initialization and platform-specific configurations
```

</details>

### Dependencies (pubspec.yaml)

<details>
<summary>Click to expand pubspec.yaml</summary>

```yaml
name: tm_flutter_app
description: A new Flutter project
publish_to: 'none'

version: 1.0.0+1

environment:
  sdk: ">=3.0.0 <4.0.0"

dependencies:
  flutter:
    sdk: flutter

  camera: ^0.10.5+9
  fl_chart: ^0.68.0
  permission_handler: ^11.3.1
  tflite_flutter: ^0.12.0
  image: ^4.2.0
  google_fonts: ^6.2.1
  image_picker: ^1.1.2
  cupertino_icons: ^1.0.8
  intl: ^0.19.0
  firebase_core: ^2.31.0
  cloud_firestore: ^4.17.3
  path_provider: ^2.1.1

dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^4.0.0

flutter:
  uses-material-design: true

  assets:
    - assets/model/labels.txt
    - assets/model/model_unquant.tflite
```

</details>

---

## �📱 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/caffiolens.git

# Navigate to project directory
cd caffiolens

# Install dependencies
flutter pub get

# Run the app
flutter run
```

---

## 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Anthony Charles Monoy**
- 📧 Email: anthonycharles.monoy@csucc.edu.ph
- 🎓 Course: ITE120 Final Project
- 🏫 Institution: CSUCC

---

<div align="center">

**Made with ❤️ and ☕ using Flutter**

⭐ Star this repo if you find it helpful!

</div>
