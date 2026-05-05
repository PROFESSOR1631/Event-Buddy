# 🗓️ EventBuddy

**EventBuddy** is a premium social platform designed to bridge the gap between digital interaction and real-world networking. Whether you're looking for a concert buddy, a workout partner, or someone to join you for an impromptu coffee, EventBuddy makes it seamless to find, create, and join real-life plans.

---

## ✨ Key Features

- 📍 **Buddy Discovery & Maps**: Integrated **Google Maps** to visualize nearby users and active plans within your vicinity.
- 💬 **Real-time Chat**: High-performance direct and group messaging powered by **Socket.io**.
- 🔔 **Smart Notifications**: Dual-layer notification system using **Firebase Cloud Messaging (FCM)** for push alerts and Socket.io for in-app updates.
- ✨ **"Midnight Luxury" UI**: A state-of-the-art dark mode design system implemented with **NativeWind (Tailwind CSS)** and **Reanimated**.
- 📸 **Social Stories**: Share your event highlights with ephemeral photo updates.
- 🔐 **Secure Auth**: Robust authentication flow featuring **Phone/OTP verification** via Firebase and JWT-protected backend routes.

---

## 🛠️ Tech Stack

### Frontend
- **Framework**: React Native (v0.81.5)
- **Styling**: NativeWind (Tailwind CSS)
- **Animations**: React Native Reanimated
- **Navigation**: React Navigation (Stack & Bottom Tabs)
- **Maps**: React Native Maps
- **State/Data**: Axios, Async Storage

### Backend
- **Runtime**: Node.js & Express
- **Database**: MongoDB (Mongoose ODM)
- **Real-time**: Socket.io
- **Notifications**: Firebase Admin SDK (FCM)
- **Images**: ImageKit.io & Multer
- **Communications**: Firebase Phone Auth (OTP Services)

---

## 🚀 Getting Started

### Prerequisites
- Node.js (>= 20.x)
- Android Studio / Xcode (for emulators)
- MongoDB Instance
- Firebase Project

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/PROFESSOR1631/Event-Buddy.git
   cd EventBuddy
   ```

2. **Backend Setup**
   ```bash
   cd Backend
   npm install
   # Create a .env file based on .env.example
   # Add your firebase-service-account.json to /config
   npm start
   ```

3. **Frontend Setup**
   ```bash
   # From root directory
   npm install
   npx react-native run-android # For Android
   # OR
   npx react-native run-ios # For iOS
   ```

---

## ⚙️ Configuration & Environment

### Backend `.env`
Ensure you have the following variables configured:
| Variable | Description |
|----------|-------------|
| `MONGODB_URI` | Your MongoDB connection string |
| `JWT_SECRET` | Secret key for token signing |
| `IMAGEKIT_PUBLIC_KEY` | Public key from ImageKit.io |
| `IMAGEKIT_PRIVATE_KEY` | Private key from ImageKit.io |
| `FIREBASE_API_KEY` | Your Firebase API Key |

> [!IMPORTANT]
> For Firebase Phone Auth to work, you must add your Android **SHA-1** fingerprint to the Firebase Console and enable the "Phone" provider. See `FIREBASE_SETUP.md` for details.

---

## 🏗️ Project Structure

```text
├── android/              # Native Android configuration
├── ios/                  # Native iOS configuration
├── Backend/              # Node.js REST API
│   ├── controllers/      # Business logic
│   ├── models/           # Mongoose schemas
│   ├── services/         # FCM, Socket, and Image services
│   └── routes/           # API endpoints
├── src/                  # React Native Source
│   ├── api/              # Axios service layers
│   ├── components/       # Reusable UI components
│   ├── screens/          # Application screens
│   └── navigation/       # Navigation configuration
└── App.js                # Application entry point
```

---

## 🎨 Design Philosophy
EventBuddy follows a **"Midnight Luxury"** aesthetic. This involves:
- Deep indigo and slate-800 backgrounds.
- High-contrast typography using specialized fonts.
- Glassmorphism effects with subtle gradients.
- Micro-interactions for every touchpoint.

---

## 🤝 Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



*Created with ❤️ by the EventBuddy Team*
