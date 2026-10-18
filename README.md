# Skyflutter Android Studio project

This package wraps the Skyflutter HTML5 game in a native Android WebView. It is a source project, not a prebuilt APK/AAB.

## Project configuration
- Application ID: `com.skyflutter.game` (change this before release if you want a different unique ID; do not change it after publishing)
- Version: 1.0.0 / versionCode 1
- Minimum Android: API 23
- Compile/target SDK: 36 (Android 16 target for Google Play submissions after Aug 31, 2026)
- Java 17
- No internet permission and no ad/analytics SDKs in this build
- Offline game assets are bundled under `app/src/main/assets`

## Build using Android Studio
1. Install Android Studio on a computer (Windows, Mac, or Linux) and install Android SDK Platform 36 and a compatible Android Gradle Plugin/Gradle version when prompted.
2. Extract this ZIP. In Android Studio choose **Open** and select the extracted `SkyflutterAndroid` folder (the folder containing `settings.gradle`).
3. Let Gradle sync. If Android Studio asks to install missing SDK components, accept.
4. Run on an Android phone with USB debugging enabled or on an emulator. Test touch controls, music, screen sizes, background/resume, and score persistence.
5. Before release, set a unique application ID and increment versionCode as appropriate. Create a signed release using **Build > Generate Signed Bundle / APK > Android App Bundle**. Create and securely back up your upload key.
6. Upload the resulting signed `.aab` to Google Play Console, complete the store listing, content rating, app access, ads declaration, target audience, Data safety, and testing requirements, then submit for review.

## Important limits
- This environment does not include the Android SDK or Gradle, so no signed APK/AAB was built or tested here.
- Google Play approval is not guaranteed. You must test the final release and complete the account-specific Play Console steps.
- Earnings are not automatic. This package has no ads yet. If you want ad revenue, integrate Google Mobile Ads/AdMob properly, disclose ads and data collection accurately, test with test ads, and follow Google Play and AdMob policies. Do not click your own live ads.
- The name and visuals are an original prototype. Check app-name availability and avoid using Flappy Bird branding/artwork or implying affiliation with another game.
