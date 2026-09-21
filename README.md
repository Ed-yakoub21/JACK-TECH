# JACK TECH Android V1

This is the Android phone version of JACK TECH, built around the same working web application used on PC.

## What is included
- Same JACK TECH interface and business modules from Sync V2 SAFE.
- Local browser storage inside Android WebView.
- Supabase synchronization using the existing Sync V2 code.
- Internet permission.
- HTTPS app-assets origin so browser fetch calls to Supabase can work without the file:// problem.
- Portrait phone layout.

## Important
This package is an Android Studio project source, not a prebuilt APK. The current build environment does not contain the Android SDK/Gradle toolchain, so an APK cannot be honestly claimed as built here.

## Build
1. Open this folder in Android Studio.
2. Let Gradle sync/download the Android Gradle Plugin and dependencies.
3. Connect an Android phone with USB debugging or start an emulator.
4. Run the `app` configuration.
5. In JACK TECH, open Synchronisation and use the same Supabase URL, publishable key and account already tested on PC.

## Supabase
Do not put a service-role/secret key in the app. Use the publishable key with RLS enabled.
