# Free Fire Tournament Hub — Android starter project

This is a native Android Java starter app for a Free Fire tournament manager.

## Included
- Admin screen to create a tournament
- Solo / Duo / Squad, maps, match types, free entry and slot limit
- Match date/time selection
- Rules, prize/reward text and custom room credentials
- Player registration with numeric UID validation
- Upcoming / Live / Completed status
- Room credentials locked until 10 minutes before the scheduled start, for registered users
- Local on-device persistence using SharedPreferences

## Build an APK
1. Install **Android Studio** on a computer.
2. Extract `FreeFireTournamentHub.zip`.
3. In Android Studio choose **Open** and select the extracted `FreeFireTournamentHub` folder.
4. Allow Gradle sync. Use JDK 17 and install Android SDK Platform 35 if prompted.
5. Choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
6. When the build finishes, click **locate**. The APK is normally at:
   `app/build/outputs/apk/debug/app-debug.apk`
7. Transfer that APK to your Android phone and install it. Only install APKs you built or trust.

## Important limitations
This is a starter/demo project, not a production tournament service.
- Data is stored only on the device. It is not shared between admin and players on different phones.
- There is no real admin login, server, cloud database, push notification, or anti-cheat verification.
- For a real public tournament, add a secure backend (for example Firebase), admin authentication, server-side UID/contact validation, registration capacity checks, and server-time-based room credential release.
- Do not publish room credentials or player contact details publicly. Use guardian-approved contact details for minors.
- Use your own authorized game branding/assets; this app is an independent community tournament tool and is not an official Garena product.
