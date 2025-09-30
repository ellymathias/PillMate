
# MedRemind - Medicine Reminder App

## Overview
MedRemind is a cross-platform mobile app built with Expo and React Native to help users manage their medications, track doses, receive reminders, and monitor refills.

## Features
- Authentication (biometrics or PIN)
- Add, update, and delete medications
- Daily schedule and progress tracking
- Push notifications for medication and refill reminders
- Calendar view for dose history
- Refill tracker
- History log (taken/missed doses)
- Themed UI (light/dark mode)

## Getting Started

### Prerequisites
- Node.js (LTS recommended)
- npm
- Expo CLI (`npm install -g expo-cli`)

### Installation
1. Clone the repository or download the source code.
2. Install dependencies:
    ```sh
    npm install --legacy-peer-deps
    ```
3. Start the development server:
    ```sh
    npx expo start
    ```

### Development Build (for notifications)
Expo Go does not support push notifications for SDK 54+. To use notifications, create a development build:
```sh
npx expo run:android   # or npx expo run:ios
```

## Project Structure
```
medicine-reminder-app-main/
   app/                # App screens and navigation
   components/         # Reusable UI components
   utils/              # Storage and notification logic
   hooks/              # Custom React hooks
   constants/          # Theme and color constants
   assets/             # Images and fonts
```

## Configuration
- Update `app.json` with your Expo project ID for push notifications:
   ```json
   {
      "expo": {
         "projectId": "your-project-id"
      }
   }
   ```

## Learn More
- [Expo Documentation](https://docs.expo.dev/)
- [React Native Documentation](https://reactnative.dev/)

## License
MIT
