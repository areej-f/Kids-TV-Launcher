# Kids-TV-Launcher

A custom launcher for Android TV designed for kids, featuring approved apps only and a PIN-protected exit.

📌 Features
✅ Displays a grid of kid-friendly apps (YouTube Kids, Netflix, etc.).
✅ Prevents access to non-approved apps.
✅ PIN-protected exit to prevent kids from leaving.
✅ Optimized for Android TV with D-pad navigation.

🛠 Tech Stack
Jetpack Compose (UI)

Kotlin (Programming Language)

Android TV SDK

PackageManager API (To list installed apps)

🚀 Installation Guide
1. Clone the Repository

git clone https://github.com/yourusername/Kids-TV-Launcher.git
cd Kids-TV-Launcher

2. Open in Android Studio
Open Android Studio.

Click File > Open, select the project folder.

3. Run on an Emulator or Device
Run on Android TV Emulator
Open AVD Manager in Android Studio.

Create a new Android TV (Google APIs) device.

Install & Run the app.

Run on a Real Android TV
Enable Developer Options on Android TV.

Connect via ADB:


adb connect <your-tv-ip>:5555
Install APK:


adb install app-debug.apk
📺 How to Use
1️⃣ Launch the app on your Android TV.
2️⃣ Navigate through the available apps using the D-pad.
3️⃣ Select an app to open it.
4️⃣ Click Exit → Enter PIN (default: 1234) to leave the launcher.

🛠 Customization
To change the approved apps, modify this list in MainActivity.kt:


val approvedApps = listOf("com.youtube.kids", "com.netflix", "com.disney.plus")
To change the PIN, update this in PINExitButton.kt:


val correctPin = "1234"
📝 License
This project is open-source under the MIT License.
