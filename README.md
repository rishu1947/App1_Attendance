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

---

## App 2 — Interactive Canvas Graphics

**Tech:** Custom View · Android Canvas API · Paint · Path · ValueAnimator · AlertDialog Quiz

### Features
- Free draw, Circle, Rectangle, Line tools
- 6 color swatches + stroke width SeekBar + fill toggle
- Animations: Bounce Ball, Rotating Shapes, Pulse Ring (all via ValueAnimator)
- Undo (bitmap snapshot history, last 20 strokes)
- Clear canvas
- Shape identification quiz (multiple choice AlertDialog)

### Setup
1. Open `App2_Canvas/` in Android Studio
2. Run ▶️ — no API keys or Firebase needed

---

## App 3 — Weather Information App

**Tech:** Retrofit 2 · OkHttp · Gson · OpenWeatherMap API · MVVM · Coroutines · Glide

### Features
- Search any city → calls `GET /weather` + `GET /forecast` via Retrofit
- Displays: temperature, feels like, humidity, wind, pressure, visibility, sunrise/sunset
- 5-day forecast horizontal RecyclerView
- Quick-city chips: Delhi, London, New York, Tokyo, Dubai
- Full HTTP error handling (401/404/429/5xx/no-internet)

### Setup
1. Register free at https://openweathermap.org/api → get API key
2. Open `App3_Weather/local.properties` (create if missing) and add:
   ```
   WEATHER_API_KEY=paste_your_key_here
   ```
3. Open `App3_Weather/` in Android Studio → Run ▶️

---

## Project Structure (each app)

```
app/src/main/
├── java/com/cse227/<appname>/
│   ├── data/
│   │   ├── model/       ← Data classes
│   │   ├── api/         ← Retrofit interface (App3)
│   │   └── repository/  ← Firebase / Retrofit calls
│   ├── viewmodel/       ← MVVM ViewModels with LiveData
│   └── ui/              ← Activities + Fragments
└── res/
    ├── layout/          ← All XML layouts
    ├── values/          ← strings.xml, themes.xml
    ├── menu/            ← BottomNav menu (App1)
    └── drawable/        ← Icons, shapes
```

## Submission Checklist
- [ ] Source Code (this ZIP)
- [ ] Screenshots of Output
- [ ] Upload to GitHub and include the link
