workflows:
  android-workflow:
    name: Build APK
    environment:
      flutter: stable
      xcode: latest
    scripts:
      - name: Install dependencies
        script: flutter pub get
      - name: Build APK
        script: flutter build apk --release
    artifacts:
      - build/app/outputs/flutter-apk/app-release.apk# Hayati-jadida
