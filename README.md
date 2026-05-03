# SAPIFY

A Spotify-inspired music streaming Android application built with Java and Firebase.

---

## Overview

SAPIFY is an Android app that brings a music streaming experience to mobile. Built as a personal project using native Android development with Java, it integrates Firebase as its backend for real-time data, authentication, and storage.

---

## Technologies

| Layer | Technology |
|-------|-----------|
| Language | Java |
| Platform | Android |
| Backend / Database | Firebase (Firestore / Realtime Database) |
| Authentication | Firebase Authentication |
| Build System | Gradle (Kotlin DSL) |
| IDE | Android Studio |

---

## Project Structure

```
SAPIFY/
├── app/                        # Main Android application module
│   ├── src/
│   │   └── main/
│   │       ├── java/           # Java source files (Activities, Fragments, etc.)
│   │       ├── res/            # Layouts, drawables, strings, and other resources
│   │       └── AndroidManifest.xml
│   └── build.gradle.kts        # App-level Gradle config
├── gradle/                     # Gradle wrapper files
├── build.gradle.kts            # Project-level Gradle config
├── settings.gradle.kts         # Project settings
└── gradle.properties           # Gradle JVM and AndroidX settings
```

---

## Getting Started

### Prerequisites

- [Android Studio](https://developer.android.com/studio) (latest stable version recommended)
- Android SDK (API level as configured in `app/build.gradle.kts`)
- A Firebase project with the `google-services.json` file

## Configuration

The project uses the following key Gradle settings (configured in `gradle.properties`):

```properties
org.gradle.jvmargs=-Xmx2048m -Dfile.encoding=UTF-8
android.useAndroidX=true
android.nonTransitiveRClass=true
```

---

## Firebase Setup

SAPIFY uses Google Firebase as its backend. Make sure the following Firebase services are enabled in your Firebase project as needed:

- **Firebase Authentication** — for user sign-in/sign-up
- **Cloud Firestore or Realtime Database** — for storing music data, playlists, and user info
- **Firebase Storage** — for storing audio files and artwork (if applicable)

> The `google-services.json` file is **not included** in this repository for security reasons. You must provide your own.

---

## Author

**Christos Sapounas**

- GitHub: [@sapounasGH](https://github.com/sapounasGH)

---

## License

This project was developed as a university project.
