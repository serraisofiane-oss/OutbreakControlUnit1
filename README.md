# Outbreak Control Unit — Android app source

This is an Android Studio project for an offline presentation viewer based on the secondary-school Outbreak Control Unit project.

## What it contains
- 13 presentation slides plus a bonus knowledge-check slide
- Fictional outbreak statistics clearly labelled as fictional
- Slide navigation and a responsive bar chart
- No network permission; the app's main presentation works offline. Source links require internet if opened.

## Build an APK
An APK could not be compiled in this environment because the Android SDK and Gradle are not installed. The source project is provided so it can be built with Android Studio.

1. Install Android Studio and its Android SDK (API 35 or compatible).
2. Open this folder (`OutbreakControlUnit_Android_Project`) in Android Studio.
3. Allow Gradle sync to complete.
4. Choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. Android Studio will show a link to the generated debug APK, usually under `app/build/outputs/apk/debug/app-debug.apk`.

The APK produced by Android Studio is a debug build suitable for testing. Do not treat the fictional scenario as a real outbreak alert or as medical advice.


## Build the APK using only your Android phone (GitHub cloud build)

This workflow lets GitHub's cloud computer build the APK. You do not need a PC, but you do need a GitHub account and an internet connection.

1. In your phone browser, sign in to GitHub and create a new empty repository.
2. Upload the contents of this project folder to the repository, including the hidden `.github/workflows/build-apk.yml` file. If the mobile upload interface hides dot-folders, switch your browser to desktop mode.
3. Open the repository's Actions tab and select **Build Outbreak Control Unit APK**. Tap **Run workflow** if it has not already started after upload.
4. Open the completed workflow run. Under Artifacts, download `Outbreak-Control-Unit-debug-apk`.
5. Extract the downloaded artifact ZIP on your phone. Open `app-debug.apk` and approve Android's install-from-this-source prompt if asked.

The workflow produces a debug APK for testing. This chat cannot upload to or operate your personal GitHub account for you.
