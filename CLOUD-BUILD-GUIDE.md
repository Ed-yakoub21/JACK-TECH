# JACK TECH — Cloud APK Build

This project is prepared to build the Android APK with GitHub Actions, so no PC/Android Studio is required for the build machine.

## Build
1. Create a GitHub repository from this folder.
2. Upload the project contents to the repository.
3. Open the repository's **Actions** tab.
4. Select **Build JACK TECH APK**.
5. Choose **Run workflow**.
6. Wait for the green check.
7. Open the workflow run and download the artifact **JACK-TECH-APK**.
8. The artifact contains `app-debug.apk`.

The workflow uses JDK 17, Gradle 8.9, Android Gradle Plugin 8.7.3, and builds `:app:assembleDebug`.

## Important
- Do not put Supabase service-role/secret keys in the repository.
- The app's existing publishable-key/local configuration remains unchanged.
- This produces a debug APK for testing. A release APK needs a signing key and release signing configuration.
