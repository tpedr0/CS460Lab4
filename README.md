# Android Firebase Authentication App

## Overview
This Android application demonstrates user authentication implementation using Firebase. The app features a modern, material design-based UI that allows users to create accounts, sign in securely, and customize their profiles with profile pictures.

## Features
- **User Authentication**
  - Email and password-based authentication
  - Form validation with toast notifications
  - Secure user session management
  
- **User Registration**
  - Profile picture upload capability
  - Password confirmation
  - Input validation with real-time feedback
  
- **Firebase Integration**
  - Secure user data storage
  - Profile image storage
  - Real-time authentication
  
- **UI/UX**
  - Material Design principles
  - Seamless navigation between sign-in and registration
  - Progress indicators during authentication
  - Toast notifications for user feedback
  - Primary color scheme: FFD83D68

## Technical Architecture
- **Frontend**: Native Android with Java
- **Backend**: Firebase Authentication & Firestore
- **Data Storage**: SharedPreferences for local storage
- **Image Processing**: Base64 encoding for profile images

## Project Structure
```
CSLab4/
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── com.example.cslab4/
│           │       ├── activities/
│           │       │   ├── MainActivity
│           │       │   ├── SignInActivity
│           │       │   └── SignUpActivity
│           │       ├── firebase/
│           │       │   └── MessagingService
│           │       └── utilities/
│           │           ├── Constants
│           │           └── PreferenceManager
│           ├── res/
│           │   ├── drawable/
│           │   │   ├── background_image.xml
│           │   │   ├── background_input.xml
│           │   │   ├── ic_launcher_background.xml
│           │   │   └── ic_launcher_foreground.xml
│           │   ├── layout/
│           │   │   ├── activity_main.xml
│           │   │   ├── activity_sign_in.xml
│           │   │   └── activity_sign_up.xml
│           │   ├── values/
│           │   │   ├── colors.xml
│           │   │   ├── strings.xml
│           │   │   └── themes/
│           │   │       ├── themes.xml
│           │   │       └── themes.xml (night)
│           │   └── mipmap/
│           └── AndroidManifest.xml
└── gradle scripts
```

## Key Components
- **SignInActivity**: Handles user authentication
- **SignUpActivity**: Manages new user registration
- **PreferenceManager**: Manages local data storage
- **MessagingService**: Handles Firebase Cloud Messaging
- **Constants**: Stores app-wide constant values

## Setup Instructions
1. Clone the repository
2. Open the project in Android Studio
3. Connect your Firebase project:
   - Add your `google-services.json` file
   - Configure Firebase Authentication
   - Set up Firestore Database
4. Build and run the application

## Dependencies
```gradle
dependencies {
    // Firebase
    implementation 'com.google.firebase:firebase-firestore'
    implementation 'com.google.firebase:firebase-messaging'
    
    // AndroidX
    implementation 'androidx.appcompat:appcompat'
    implementation 'androidx.activity:activity'
}
```

## Implementation Details
- User authentication is handled through Firebase Authentication
- User data and profile images are stored in Firebase Firestore
- Local session management using SharedPreferences
- Form validation ensures data integrity before submission
- Toast notifications provide user feedback for all actions

## Documentation
All methods are documented using Javadoc format for better code maintainability and understanding. Key documentation includes:
- Method parameters and return values
- Function purposes and behaviors
- Class-level documentation
- Constants documentation

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is created as part of an academic assignment.

## Acknowledgments
- Firebase Documentation
- Android Developer Documentation
- Material Design Guidelines
