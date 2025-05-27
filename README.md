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
2.  **Build**:
    * Open the project in Android Studio.
    * In the `iosApp` directory, run `pod install`.
    * Either open the generated `.xcworkspace` in Xcode and run on a simulator or device, or run the iosApp target in Android Studio with the run configuration set to use the generated `.xcworkspace`.
