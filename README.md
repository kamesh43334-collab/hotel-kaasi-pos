# Hotel Kaasi POS — Android & iOS app project

This project wraps the existing `index.html` POS application using Capacitor.

## Requirements
- Node.js (LTS)
- Android Studio + Android SDK for Android builds
- macOS + Xcode for iOS builds (Apple requires Xcode to compile/sign iOS apps)

## Setup
```bash
npm install
npx cap add android
npx cap add ios
npx cap sync
```

## Open native projects
```bash
npm run android
npm run ios
```

Build and run from Android Studio or Xcode. For store release, configure app icons,
launch screens, signing certificates, privacy details, and store listings.

## Important notes
- The app's existing HTML/CSS/JavaScript is in `www/index.html`.
- The current HTML uses some CDN-hosted libraries/fonts, so those features may need
  internet access unless the libraries are bundled locally.
- Existing browser/local storage is device-local. It does not automatically sync
  bills or settings between multiple phones. A secure cloud database and login system
  are needed for shared multi-device records.
- iOS builds must be compiled and signed on macOS using Xcode.
