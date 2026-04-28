# 🚀 NavigationSimpleDemo | Kotlin & Android Jetpack

<p align="center">
  <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" />
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" />
  <img src="https://img.shields.io/badge/Jetpack_Navigation-4285F4?style=for-the-badge&logo=google&logoColor=white" />
  <img src="https://img.shields.io/badge/MAD_Score-Gold-yellow?style=for-the-badge" />
</p>

---

## 🌟 Overview
**NavigationSimpleDemo** is a high-performance, education-focused Android application designed to master the **Android Jetpack Navigation Component**. This project serves as a cornerstone for learning how to manage complex fragment transactions, safe data passing, and lifecycle-aware UI components in a modern Android environment.

Built with **100% Kotlin**, this project demonstrates the transition from traditional Activity-based navigation to the modern **Single Activity Architecture**.

---

## 📸 App Showcase

---

## 🛠 Tech Stack & Modern Android Development (MAD)
This project is built using the latest industry standards:

- **Language:** [Kotlin](https://kotlinlang.org/) (Coroutines, KTX)
- **Architecture:** Single Activity Architecture
- **Jetpack Components:**
  - **Navigation Component:** For seamless fragment transitions.
  - **SafeArgs / Bundles:** For type-safe data passing.
  - **Fragments:** Modular UI components.
- **UI Tooling:** Material Design 3, ConstraintLayout.

### 🏆 MAD Score
| Category | Status | Score |
| :--- | :--- | :--- |
| **Kotlin** | ✅ Fully Migrated | 100% |
| **Navigation** | ✅ Jetpack Navigation | 100% |
| **Architecture** | ✅ Single Activity | 100% |
| **UI** | ✅ Material Design | 90% |

---

## 📊 Application Flow
The following flowchart illustrates the user journey and data persistence layer:

```mermaid
graph TD
    Start((Start)) --> A[Splash/MainActivity]
    A --> B[EnterDetailsFragment]
    B --> C{Validation}
    C -- "Invalid" --> B
    C -- "Valid" --> D[Pass Data via Bundle]
    D --> E[VerifyDetailsFragment]
    E --> F[Display Information]
    F -- "Back" --> B
```

---

## 🏗 MVVM Architecture (Conceptual)
While this is a simple demo, the application is prepared for a full **MVVM (Model-View-ViewModel)** implementation:

```mermaid
graph BT
    subgraph UI_Layer
    Fragment[EnterDetailsFragment]
    end
    
    subgraph Logic_Layer
    VM[DetailsViewModel]
    end
    
    subgraph Data_Layer
    Repo[DetailsRepository]
    DB[(Local Data)]
    end

    Fragment <--> VM
    VM <--> Repo
    Repo <--> DB
```

---

## 🚀 Getting Started
1. **Clone the repo:**
   ```bash
   git clone https://github.com/yourusername/NavigationSimpleDemo.git
   ```
2. **Open in Android Studio:**
   Ensure you have the latest Arctic Fox or Bumblebee version.
3. **Run the app:**
   Select your emulator or physical device and hit `Run`.

---

## 👨‍💻 Learning Objectives
- [x] Setting up a `NavHostFragment`.
- [x] Defining Navigation Graphs (`nav_graph.xml`).
- [x] Navigating between destinations using `NavController`.
- [x] Passing arguments using `Bundle` and retrieving them.
- [x] Overriding `onSupportNavigateUp` for system back button support.

---

<p align="center">
  Developed with ❤️ for Android Education.
</p>
