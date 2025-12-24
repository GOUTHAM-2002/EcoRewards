# 🌱 EcoRewards - Gamify Your Green Impact

**Turn everyday eco-friendly actions into rewards.** Track, earn, and redeem points for creating a cleaner, greener planet.

![Flutter](https://img.shields.io/badge/Flutter-3.0+-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

---

## 🌍 About

**EcoRewards** is a mobile application that incentivizes sustainable living by rewarding users with redeemable points for every eco-friendly action they take. From recycling to using public transport, every small action counts toward a cleaner environment—and earns you rewards!

Built with **Flutter** for cross-platform compatibility and powered by **Firebase** for real-time data synchronization.

---

## ✨ Key Features

### 🎯 Track Your Impact
- Log eco-friendly activities (recycling, carpooling, using reusable bags, etc.)
- View your carbon footprint reduction in real-time
- Track daily, weekly, and monthly sustainability goals

### 💰 Earn EcoPoints
- Receive points for verified green actions
- Complete daily challenges and missions
- Unlock achievements and badges
- Climb the leaderboard and compete with friends

### 🎁 Redeem Rewards
- Exchange points for real-world rewards
- Partner with local businesses and brands
- Get discounts on eco-friendly products
- Donate points to environmental causes

### 📊 Analytics & Insights
- Visualize your environmental impact
- See how your actions contribute to global sustainability
- Get personalized recommendations for greener living
- Compare your progress with the community

### 🤝 Community & Social
- Share achievements on social media
- Join community challenges
- Connect with like-minded eco-warriors
- Create teams and compete together

---

## 📱 Screenshots

> *Coming soon -  app screenshots here*

<table>
  <tr>
    <td><img src="screenshots/home.png" width="250" alt="Home Screen"/></td>
    <td><img src="screenshots/activities.png" width="250" alt="Activities"/></td>
    <td><img src="screenshots/rewards.png" width="250" alt="Rewards"/></td>
  </tr>
  <tr>
    <td align="center">Home Screen</td>
    <td align="center">Log Activities</td>
    <td align="center">Redeem Rewards</td>
  </tr>
</table>

---

## 🚀 Getting Started

### Prerequisites

- **Flutter SDK** (3.0 or higher) - [Install Flutter](https://docs.flutter.dev/get-started/install)
- **Dart SDK** (2.19 or higher)
- **Android Studio** / **Xcode** (for device testing)
- **Firebase Account** - [Firebase Console](https://console.firebase.google.com/)

### Installation

1. **Clone the repository**
```bash
   git clone https://github.com/GOUTHAM-2002/EcoRewards.git
   cd EcoRewards
```

2. **Install dependencies**
```bash
   flutter pub get
```

3. **Configure Firebase**
   - Create a new Firebase project
   - Add Android and iOS apps to your Firebase project
   - Download `google-services.json` (Android) and `GoogleService-Info.plist` (iOS)
   - Place them in the appropriate directories:
     - Android: `android/app/google-services.json`
     - iOS: `ios/Runner/GoogleService-Info.plist`

4. **Run the app**
```bash
   # Check connected devices
   flutter devices
   
   # Run on your device/emulator
   flutter run
```

---

## 🏗️ Project Structure
```
EcoRewards/
├── android/              # Android-specific files
├── ios/                  # iOS-specific files
├── lib/                  # Main application code
│   ├── models/          # Data models
│   ├── screens/         # UI screens
│   ├── widgets/         # Reusable widgets
│   ├── services/        # API & Firebase services
│   ├── utils/           # Helper functions
│   └── main.dart        # App entry point
├── assets/              # Images, fonts, etc.
├── web/                 # Web platform files
├── linux/               # Linux platform files
├── macos/               # macOS platform files
├── windows/             # Windows platform files
├── pubspec.yaml         # Dependencies
└── README.md            # You are here
```

---

## 🛠️ Built With

- **[Flutter](https://flutter.dev/)** - Cross-platform UI framework
- **[Dart](https://dart.dev/)** - Programming language
- **[Firebase](https://firebase.google.com/)** - Backend services
  - Firebase Authentication
  - Cloud Firestore
  - Firebase Storage
  - Firebase Analytics
- **[Provider](https://pub.dev/packages/provider)** - State management
- **[Google Maps API](https://developers.google.com/maps)** - Location services (optional)

---

## 🎮 How It Works

### 1. Sign Up & Create Profile
- Register with email or social login
- Set your sustainability goals
- Complete your profile

### 2. Log Eco-Actions
- Select from predefined activities or add custom ones
- Upload proof (photos, receipts) for verification
- Get instant EcoPoints credited

### 3. Complete Challenges
- Daily missions (e.g., "Use public transport today")
- Weekly challenges (e.g., "Recycle 5 items this week")
- Special events and campaigns

### 4. Redeem Rewards
- Browse available rewards in the marketplace
- Redeem points for discounts, vouchers, or donations
- Track your redemption history

---

## 🌟 EcoActions Examples

| Action | Points | Verification |
|--------|--------|--------------|
| Recycle plastic bottle | 10 | Photo of recycling bin |
| Use public transport | 25 | GPS check-in |
| Plant a tree | 100 | Photo + location |
| Use reusable bag | 5 | Photo of shopping |
| Carpool to work | 30 | GPS tracking |
| Compost food waste | 20 | Photo proof |
| Buy eco-friendly products | 50 | Receipt scan |

---

## 🔐 Firebase Setup

### Required Firebase Services

1. **Authentication**
   - Enable Email/Password authentication
   - Optional: Google, Facebook sign-in

2. **Firestore Database**
   - Create collections: `users`, `activities`, `rewards`, `challenges`
   - Set up security rules

3. **Storage**
   - Configure for photo uploads
   - Set storage rules

4. **Analytics** (Optional)
   - Track user engagement
   - Monitor app performance

### Firestore Structure
```
users/
  ├── {userId}/
      ├── profile
      ├── totalPoints
      ├── activities []
      └── achievements []

activities/
  ├── {activityId}/
      ├── userId
      ├── type
      ├── points
      ├── timestamp
      └── verified

rewards/
  ├── {rewardId}/
      ├── name
      ├── description
      ├── pointsCost
      └── available

challenges/
  ├── {challengeId}/
      ├── title
      ├── pointsReward
      ├── startDate
      └── endDate
```

---

## 🎯 Roadmap

### Phase 1: MVP (Current)
- [x] User authentication
- [x] Basic activity logging
- [x] Points system
- [x] Simple rewards catalog

### Phase 2: Enhancement
- [ ] Social features (friends, groups)
- [ ] Advanced analytics dashboard
- [ ] Push notifications for challenges
- [ ] QR code scanning for rewards

### Phase 3: Scale
- [ ] AI-powered recommendations
- [ ] Corporate partnerships
- [ ] Blockchain-based carbon credits
- [ ] AR features for gamification
- [ ] Multi-language support

### Phase 4: Expansion
- [ ] Web platform
- [ ] Desktop applications
- [ ] Integration with smart home devices
- [ ] API for third-party apps

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Areas We Need Help With
- UI/UX improvements
- New eco-action ideas
- Bug fixes and testing
- Documentation
- Translation to other languages

---

## 🐛 Bug Reports & Feature Requests

Found a bug or have an idea? Open an issue on GitHub!

- **Bug Report**: Include steps to reproduce, expected vs actual behavior
- **Feature Request**: Describe the feature and its use case

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🌍 Our Mission

**Making sustainability fun, accessible, and rewarding for everyone.**

Climate change is real, and every action counts. EcoRewards makes it easy and rewarding to make sustainable choices in your daily life. Together, we can create a cleaner, greener planet—one action at a time.

---

## 📊 Impact So Far

> *These will be real metrics once the app launches*

- 🌱 **0+** Trees planted
- ♻️ **0+** Items recycled
- 🚗 **0+** Miles saved by carpooling
- 🌍 **0+** Tons of CO₂ reduced

---

## 👥 Team

**Goutham N** - *Creator & Developer*
- GitHub: [@GOUTHAM-2002](https://github.com/GOUTHAM-2002)
- Email: goutham3336@gmail.com

---

## 🙏 Acknowledgments

- Thanks to the Flutter community for amazing resources
- Environmental organizations inspiring this project
- Early testers and supporters
- Open-source contributors

---

## 📞 Contact & Support

- **Email**: goutham3336@gmail.com
- **GitHub Issues**: [Report bugs or request features](https://github.com/GOUTHAM-2002/EcoRewards/issues)

---

## 🌟 Show Your Support

If you believe in sustainable living and want to support this project:

- ⭐ **Star** this repository
- 🍴 **Fork** it to contribute
- 📢 **Share** with friends who care about the environment
- 💚 **Spread the word** about sustainable living

---

## 📱 Download

> *Coming soon to App Store and Google Play*

[![Google Play](https://img.shields.io/badge/Google_Play-Coming_Soon-414141?style=for-the-badge&logo=google-play&logoColor=white)](#)
[![App Store](https://img.shields.io/badge/App_Store-Coming_Soon-0D96F6?style=for-the-badge&logo=app-store&logoColor=white)](#)

---

**Together, let's make every day Earth Day! 🌍💚**

---

*"The greatest threat to our planet is the belief that someone else will save it." - Robert Swan*
