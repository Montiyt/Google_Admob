AdMob Lottie App

A Flutter application demonstrating AdMob Interstitial and Native Ads with a Lottie animation on the splash screen.

Features





Splash Screen: Displays a 4-second Lottie progress bar animation, loads Interstitial and Native Ads (max 8 seconds), and handles network unavailability.



Main Screen: Displays the Native Ad and handles app lifecycle events (e.g., showing Interstitial Ad on resume).



Ad Handling: Uses google_mobile_ads for AdMob integration.



Network Handling: Uses connectivity_plus to check network status.



Animations: Uses lottie for a smooth progress bar animation.

Prerequisites





Flutter SDK (3.0.0 or later)



VS Code with Flutter and Dart extensions



Android Studio or emulator/physical device



AdMob account with App ID and Ad Unit IDs



Lottie animation file (progress.json)

Setup Instructions





Clone the Repository:

git clone <repository-url>
cd admob_lottie_app



Install Dependencies:

flutter pub get



Add AdMob IDs:





Update android/app/build.gradle with your AdMob App ID.



Update android/app/src/main/AndroidManifest.xml with your AdMob App ID.



Update lib/main.dart and lib/main_screen.dart with your Interstitial and Native Ad Unit IDs.



Add Lottie Animation:





Place your progress.json file in assets/animations/.



Run the App:

flutter run

Dependencies





google_mobile_ads: ^5.1.0



lottie: ^3.1.2



connectivity_plus: ^6.0.5

Notes





Ensure an active internet connection for ad loading.



Use test AdMob IDs for development (replace with real IDs for production).



The Lottie animation should be 4 seconds long.

Testing





Test with and without network connectivity.

A little bit issue is there that after running the spalash screen, the interstitial ad is not visible.



Test ad loading success and failure.



Test app minimization and resumption.
