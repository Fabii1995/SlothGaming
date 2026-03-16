# SlothGaming 🦥🎮

**SlothGaming** is a modern Android application designed for gamers to discover, review, and track their favorite titles. This project serves as a bridge between high-quality game metadata and a personalized user community.

> [!IMPORTANT]
> **Server Wake-up Note:** The backend for this project is hosted on a **Render Free Plan**. If the app hasn't been used recently, the server will be in "sleep mode." Please allow **1–2 minutes** for the server to wake up during the first request after launch.

---

## 🚀 Features
* **Game Discovery:** Browse top-rated titles, upcoming releases, and publisher spotlights.
* **Personalized Reviews:** Full CRUD functionality to write, edit, and delete your own game reviews.
* **Real-time Auth:** Secure user registration and login powered by Firebase.
* **Offline Support:** Local persistence ensures you can view your reviews and cached game data without an internet connection.

---

## 🛠 Tech Stack
* **Language:** [Kotlin](https://kotlinlang.org/)
* **UI Framework:** [Jetpack Compose](https://developer.android.com/jetpack/compose) (Modern, declarative UI)
* **Architecture:** MVVM (Model-View-ViewModel) for clean separation of concerns
* **Local Database:** Room for robust local persistence
* **Networking:** Retrofit & OkHttp for API communication with the IGDB database
* **Dependency Injection:** Hilt/Dagger for modular and testable code
* **Backend/Auth:** Firebase Authentication and Firestore
* **Asynchrony:** Coroutines & Kotlin Flows (StateFlow/SharedFlow) for smooth, non-blocking UI

---

## 🏗 Architecture
The project follows **Modern Android Development (MAD)** guidelines:
1. **UI Layer:** Jetpack Compose with State Hoisting to ensure the UI is a direct reflection of the state.
2. **Domain Layer:** ViewModels handle business logic and expose data via `StateFlow`.
3. **Data Layer:** A Repository pattern manages data from two sources: the local Room database and the remote IGDB API.

---

## 📸 Screenshots
| Home Screen | Game Details | My Reviews |
| :---: | :---: | :---: |
| *Add Image Link Here* | *Add Image Link Here* | *Add Image Link Here* |

---

## ⚙️ Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/YourUsername/SlothGaming.git](https://github.com/YourUsername/SlothGaming.git)
2. Open the project in Android Studio.

3. Connect your Firebase project and add the google-services.json file to the app/ directory.

4. Build and run on a physical device or emulator.
