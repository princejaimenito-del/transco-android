# TransCo — Android app (APK)

Android shell (WebView) for the live TransCo web system. Passengers, drivers and admins log in with the same accounts as the website. Supports GPS (driver tracking / passenger location), ID photo upload, PayPal checkout, pull-to-refresh and offline message.

## Get the APK — no Android Studio needed (GitHub)
1. Create a new GitHub repository and upload everything in this folder (keep the `.github` folder).
2. Open **Actions → Build TransCo APK → Run workflow**, type your live site address (e.g. `https://yourdomain.com/transco/`), click Run.
3. After ~5 minutes, open the finished run and download **TransCo-APK** → `app-debug.apk`.
4. Copy the APK to the phone, open it and allow "Install unknown apps".

## Or build with Android Studio
1. Open this folder in Android Studio (Hedgehog or newer). 
2. Edit `TRANSCO_URL` in `gradle.properties` to your live site address.
3. **Build → Build APK(s)**. File: `app/build/outputs/apk/debug/app-debug.apk`.

Note: GPS sharing continues only while the app is open on screen (keep the driver's screen on during a trip).
