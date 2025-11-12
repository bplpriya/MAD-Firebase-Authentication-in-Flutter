
# Firebase Auth Demo - Flutter

This Flutter project demonstrates **Firebase Authentication** using Email & Password.  
It includes separate screens for **Login, Registration, and Profile**.

---

## Features

- Register new users (email & password, password ≥ 6 characters)
- Sign in existing users
- Profile screen shows logged-in user's email
- Change password (send password reset email)
- Logout and return to login screen
- Firebase initialized properly

---

## Screens

1. **Login Screen** (`login_screen.dart`)
2. **Register Screen** (`register_screen.dart`)
3. **Profile Screen** (`profile_screen.dart`)

---

## Setup Instructions

1. Clone or download this repository.
2. Run:

```bash
flutter pub get
```

3. Add Firebase:

```bash
flutterfire configure
```

- Select your Firebase project
- Select Android (and Web if you want Chrome support)
  
  Add Dependencies:

Modify your pubspec.yaml file to include the necessary Firebase dependencies.

flutter pub add firebase_auth

flutter pub add firebase_core

4. Place `google-services.json` inside:

```
android/app/google-services.json
```

5. Run the app:

```bash
flutter run
```

- For Android device/emulator: `flutter run -d emulator-5554`
- For Chrome (Web): `flutter run -d chrome`

6. Build APK for submission:

```bash
flutter build apk --release
```

APK will be at:

```
build/app/outputs/flutter-apk/app-release.apk
```

---

## Dependencies

```yaml
dependencies:
  flutter:
    sdk: flutter
  firebase_core: latest
  firebase_auth: latest
  cloud_firestore: latest
```
