# ☕ CaffioLens - Coffee Pack Identifier

<div align="center">

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)

**An intelligent Flutter mobile application that uses AI to identify and classify coffee packs through camera scanning**

[Features](#-features) • [Screenshots](#-screenshots) • [Installation](#-installation) • [Tech Stack](#-tech-stack) • [Usage](#-usage)

</div>

---

## 🌟 Features

- 📷 **Real-time Camera Scanning** - Instantly scan coffee packs using your device camera
- 🤖 **AI-Powered Recognition** - TensorFlow Lite model for accurate coffee pack identification
- 📊 **Analytics Dashboard** - Track scan statistics, success rates, and scanning trends
- 🔍 **Gallery Integration** - Pick and analyze images from your device gallery
- 📜 **Scan History** - Browse and manage all your previous scans with Firebase storage
- 🎨 **Modern UI/UX** - Beautiful coffee-themed design with smooth animations
- 📈 **Real-time Stats** - Monitor total scans, success rate, and today's scans
- ☁️ **Cloud Sync** - Firebase Firestore integration for data persistence

---

## 📱 Screenshots

<div align="center">

### Home Screen
![Home Screen](https://raw.githubusercontent.com/yourusername/caffiolens/main/screenshots/home_screen.png)

Displays scan statistics and recent scan history with a clean, modern interface.

---

### Camera Scanning
![Camera Screen](https://raw.githubusercontent.com/yourusername/caffiolens/main/screenshots/camera_screen.png)

Real-time camera preview for scanning coffee packs with intuitive controls.

---

### Scan Results
![Results Screen](https://raw.githubusercontent.com/yourusername/caffiolens/main/screenshots/results_screen.png)

Detailed results showing identified coffee pack with confidence level.

---

### Scan History
![History Screen](https://raw.githubusercontent.com/yourusername/caffiolens/main/screenshots/history_screen.png)

Browse all your previous scans with filtering and search capabilities.

</div>

---

## 🚀 Installation

### Prerequisites

- **Flutter SDK** >= 3.0.0
- **Dart SDK** >= 3.0.0
- **Android Studio** / **Xcode** (for mobile development)
- **Firebase Account** (for cloud features)

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/caffiolens.git
   cd caffiolens
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

3. **Configure Firebase**
   - Create a new Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Add your Android/iOS app to the Firebase project
   - Download `google-services.json` (Android) or `GoogleService-Info.plist` (iOS)
   - Place the configuration files in the appropriate directories
   - Run FlutterFire CLI configuration:
     ```bash
     flutterfire configure
     ```

4. **Add TensorFlow Lite Model**
   - Place your trained model files in `assets/model/`:
     - `model_unquant.tflite`
     - `labels.txt`

5. **Run the app**
   ```bash
   flutter run
   ```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **Flutter** | Cross-platform mobile framework |
| **Dart** | Programming language |
| **TensorFlow Lite** | On-device machine learning inference |
| **Firebase Firestore** | Cloud database for scan history |
| **Firebase Core** | Firebase initialization and configuration |
| **Camera Plugin** | Access device camera for scanning |
| **Image Picker** | Gallery image selection |
| **FL Chart** | Beautiful charts for analytics |
| **Google Fonts** | Modern typography (Lato font) |
| **Permission Handler** | Runtime permissions management |

---

## 📖 Usage

### Scanning Coffee Packs

1. **Launch the app** and grant camera permissions when prompted
2. **Navigate to "Scan Image"** using the bottom navigation
3. **Point your camera** at a coffee pack
4. **Tap the capture button** to take a photo
5. **View the results** showing the identified coffee type and confidence level
6. **Results are automatically saved** to your scan history

### Picking from Gallery

1. **Tap "Pick Gallery"** in the navigation bar
2. **Select an image** from your device
3. **View the analysis results** instantly
4. **History entry is created** automatically

### Viewing History

1. **Navigate to "History"** tab
2. **Browse all your scans** with timestamps and confidence levels
3. **Filter scans** by success status
4. **Tap any scan** to view detailed information

### Dashboard Analytics

The home screen displays:
- **Total Scans**: All-time scan count
- **Success Rate**: Percentage of successfully identified packs
- **Today's Scans**: Number of scans performed today
- **Recent Scans**: Last 10 scans with preview cards

---

## 🎨 Color Scheme

The app uses a professional coffee-themed color palette:

- **Primary Brown**: `#6D4C41` - Main brand color
- **Light Brown**: `#8D6E63` - Secondary elements
- **Dark Brown**: `#4E342E` - Text and accents
- **Success Green**: `#388E3C` - Successful scans
- **Warning Orange**: `#D84315` - Failed scans
- **Background**: `#F5F5F5` - Clean, modern base

---

## 📂 Project Structure

```
caffiolens/
├── lib/
│   ├── main.dart                 # App entry point and main screens
│   ├── tflite_helper.dart        # TensorFlow Lite integration
│   └── firebase_options.dart     # Firebase configuration
├── assets/
│   └── model/
│       ├── model_unquant.tflite  # TensorFlow Lite model
│       └── labels.txt            # Coffee pack labels
├── android/                      # Android-specific files
├── ios/                         # iOS-specific files
├── web/                         # Web-specific files
└── pubspec.yaml                 # Dependencies and assets
```

---

## 🔒 Permissions

### Android (`AndroidManifest.xml`)
- Camera access
- Storage access (for saving scans)
- Internet (for Firebase)

### iOS (`Info.plist`)
- NSCameraUsageDescription
- NSPhotoLibraryUsageDescription

---

## 🌐 Platform Support

| Platform | Status | Notes |
|----------|--------|-------|
| **Android** | ✅ Fully Supported | Minimum SDK 21 (Android 5.0) |
| **iOS** | ✅ Fully Supported | iOS 11.0+ |
| **Web** | ⚠️ Partial Support | Camera access limited by browser |
| **Windows** | 🚧 In Development | Basic functionality |
| **macOS** | 🚧 In Development | Basic functionality |
| **Linux** | 🚧 In Development | Basic functionality |

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Your Name**

- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your Name](https://linkedin.com/in/yourprofile)
- Email: your.email@example.com

---

## 🙏 Acknowledgments

- **Flutter Team** - For the amazing cross-platform framework
- **TensorFlow Team** - For TensorFlow Lite mobile ML
- **Firebase Team** - For backend infrastructure
- **Coffee Community** - For inspiration ☕

---

<div align="center">

**Made with ❤️ and ☕**

⭐ Star this repo if you found it helpful!

</div>
