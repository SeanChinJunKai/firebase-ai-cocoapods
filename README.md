This is a Kotlin Multiplatform project targeting Android, iOS. It is a sample app showcasing [firebase-ai-kmp](https://github.com/SeanChinJunKai/firebase-ai-kmp) with Cocoapods Integration

## Key Setup
* **`:composeApp/build.gradle.kts`**:
    * Kotlin iOS targets
    * `cocoapods` block configuration for iOS
    * Firebase AI KMP SDK dependency
* **`iosApp/iosApp/iOSApp.swift`**:
    * Configures the FirebaseApp for iOS

## Running

1.  **Prerequisites**: 
    * [Environment Setup](https://www.jetbrains.com/help/kotlin-multiplatform-dev/quickstart.html#set-up-the-environment)
2.  **Firebase Console Setup**:
    * Create a Firebase Project
    * Click on AI Logic in Project Shortcuts on the left navigation sidebar
    * Enable both Gemini Developer API and Vertex AI Gemini API
    * Create an iOS app with Apple bundle ID as io.github.seanchinjunkai.firebase-ai-cocoapods
    * Download the config file `GoogleService-Info.plist` and place it in `iosApp/iosApp` directory
    * Create an Android app io.github.seanchinjunkai
    * Download the config file `google-services.json` and place it in `composeApp` directory
4.  **Build**:
    * Open the project in Android Studio.
    * In the `iosApp` directory, run `pod install`.
    * Either open the generated `.xcworkspace` in Xcode and run on a simulator or device, or run the iosApp target in Android Studio with the run configuration set to use the generated `.xcworkspace`.
