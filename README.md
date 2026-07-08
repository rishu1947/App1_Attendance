# CSE227 – Advanced Android App Development
## Assignment No. 1 — Kotlin Android Apps

---

## App 1 — Student Attendance Management

**Tech:** Firebase Authentication · Firebase Realtime Database · FCM Push Notifications · MVVM · Coroutines · Flow

### Features
- Register / Login via Firebase Auth
- Mark attendance: Present / Absent / Late
- View all records with real-time Firebase sync
- Toggle or Delete any record (CRUD)
- Subscribe to FCM push notification topic

### Setup
1. Go to https://console.firebase.google.com → create project
2. Add Android app with package `com.cse227.attendance`
3. Download `google-services.json` → paste into `App1_Attendance/app/`
4. Enable **Email/Password** under Authentication → Sign-in method
5. Enable **Realtime Database** → start in test mode
6. Open in Android Studio → Run ▶️
