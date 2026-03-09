# React Native Firebase Authentication App

A React Native mobile application built with Expo featuring Firebase Authentication.

## Features

- **User Authentication**: Sign up and Login using email and password
- **Firebase Integration**: Using Firebase Authentication v9 modular SDK
- **React Navigation**: Stack Navigator for seamless navigation
- **Clean UI**: Modern, minimal design with centered forms

## Screens

1. **Login Screen**: Email/password authentication
2. **Sign Up Screen**: Create new account with name, email, password
3. **Home Screen**: Welcome message, user email display, and logout functionality

## Project Structure

```
auth/
├── App.js                          # Main app entry point
├── src/
│   ├── config/
│   │   └── firebaseConfig.js       # Firebase configuration
│   ├── navigation/
│   │   └── AppNavigator.js         # Stack navigation setup
│   └── screens/
│       ├── LoginScreen.js          # Login screen
│       ├── SignupScreen.js         # Sign up screen
│       └── HomeScreen.js           # Home screen after login
├── .env.example                    # Example environment variables
└── package.json                    # Dependencies
```

## Prerequisites

- Node.js installed
- Expo CLI
- Firebase project with Email/Password authentication enabled

## Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file based on `.env.example`:
   ```bash
   cp .env.example .env
   ```

4. Add your Firebase credentials to `.env`:
   ```
   FIREBASE_API_KEY=your_api_key
   FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
   FIREBASE_PROJECT_ID=your_project_id
   FIREBASE_STORAGE_BUCKET=your_project.appspot.com
   FIREBASE_MESSAGING_SENDER_ID=your_sender_id
   FIREBASE_APP_ID=your_app_id
   ```

5. Run the app:
   ```bash
   npx expo start
   ```

## Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com)
2. Create a new project
3. Enable Email/Password authentication in Authentication section
4. Get your configuration from Project Settings
5. Update the `.env` file with your credentials

## Dependencies

- firebase
- @react-navigation/native
- @react-navigation/native-stack
- react-native-screens
- react-native-safe-area-context
- expo-dotenv

## License

MIT

