# 📝 Note App

[![Flutter](https://img.shields.io/badge/Flutter-3.22-blue?logo=flutter)](https://flutter.dev)
[![Dart](https://img.shields.io/badge/Dart-3.4-0175C2?logo=dart)](https://dart.dev)
[![Material%203](https://img.shields.io/badge/Material_3-Enabled-7C4DFF)](https://m3.material.io/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Android%20%7C%20iOS%20%7C%20Web%20%7C%20Desktop-lightgrey)](https://flutter.dev)

> A modern, cross-platform note-taking application built with Flutter and Material 3. Clean, fast, and built to scale.

---

## 🧠 About The Project

**Note App** is a cross-platform note-taking application built from the ground up using Flutter and Material 3 design guidelines. It aims to provide a seamless, minimal, and responsive experience across Android, iOS, Web, Linux, macOS, and Windows — all from a single codebase.

Whether you're a student jotting down lecture notes, a professional organizing tasks, or a developer looking for a clean Flutter reference project, Note App offers a solid foundation with room to grow.

> **Current status:** Active development — foundational architecture is in place, and feature work is underway.

---

## ✨ Key Features

| Area | Current | Roadmap |
|------|---------|---------|
| **UI** | Material 3 theming, responsive Scaffold | Rich text editor, dark mode toggle |
| **Platform** | Android, iOS, Web, Desktop | Platform-adaptive input |
| **State** | `StatefulWidget` + `setState` | Riverpod / BLoC integration |
| **Data** | In-memory (prototype) | Local persistence (Hive/Drift) + Cloud sync |
| **Testing** | Widget smoke test | Unit tests, integration tests, golden tests |

### Planned highlights 🚀

- 📝 Rich text note editor with markdown support
- 🏷️ Tags, categories & search
- 🔐 Biometric lock for private notes
- ☁️ Cloud sync (Firebase / Supabase)
- 📱 Offline-first architecture
- 🖨️ Export to PDF / Markdown / TXT

---

## 🏗️ Architecture & Tech Stack

### Built With

| Layer | Technology |
|-------|-----------|
| **Framework** | [Flutter](https://flutter.dev) (3.22+) |
| **Language** | [Dart](https://dart.dev) (3.4+) |
| **Design System** | Material 3 (`useMaterial3: true`) |
| **Linting** | `flutter_lints` — strict mode |
| **Testing** | `flutter_test` (widget & unit) |
| **Icons** | Material Icons + Cupertino Icons |

### Architecture Pattern

The project follows a straightforward **feature-first** layout inside `lib/`:

```
lib/
└── main.dart           # App entrypoint & route config
```

As the project grows, each feature will live in its own subdirectory with a clear separation of concerns:

```
lib/
├── core/               # Shared utilities, theme, constants
├── features/
│   ├── notes/          # Notes CRUD — UI, logic, data
│   └── settings/       # App settings screen
└── main.dart
```

> **No code generation** (freezed, json_serializable, retrofit) — all Dart is hand-written for clarity and maintainability.

---

## 🚀 Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (3.22.x or later)
- Dart 3.4+ (bundled with Flutter)
- A code editor (VS Code, Android Studio, or IntelliJ)
- An emulator / physical device (for mobile runs)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/note_app.git
cd note_app

# 2. Install dependencies
flutter pub get

# 3. Run static analysis (optional, recommended)
flutter analyze

# 4. Run tests
flutter test

# 5. Launch the app
flutter run
```

To target a specific platform:

```bash
flutter run -d chrome       # Web
flutter run -d windows      # Windows Desktop
flutter run -d macos        # macOS
flutter run -d linux        # Linux
flutter run -d emulator-5554 # Android emulator
flutter run -d ios          # iOS simulator (macOS only)
```

### Verify Your Setup

The default counter app should build and run successfully. Once confirmed, you're ready to start contributing features.

---

## 📸 Screenshots / Demo

*Screenshots and a demo video will be added here once the UI reaches a stable milestone.*

<!-- Replace these placeholders when ready -->
<p align="center">
  <img src="screenshots/home.png" alt="Home Screen" width="250"/>
  <img src="screenshots/editor.png" alt="Note Editor" width="250"/>
  <img src="screenshots/search.png" alt="Search" width="250"/>
</p>

---

## 🤝 Contributing

Contributions are what make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. 🍴 Fork the Project
2. 🌿 Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. ✅ Run `flutter analyze` and `flutter test` before committing
4. 💾 Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
5. 🚀 Push to the Branch (`git push origin feature/AmazingFeature`)
6. 🔧 Open a Pull Request

---

## 📬 Contact & Support

<div align="center">

**Your Name** &nbsp;·&nbsp; [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin)](https://linkedin.com/in/your-profile) &nbsp;·&nbsp; [![Email](https://img.shields.io/badge/Email-Contact-EA4335?logo=gmail)](mailto:your.email@example.com)

**Project Link:** [https://github.com/your-username/note_app](https://github.com/your-username/note_app)

</div>

---

<div align="center">
  <sub>Built with ❤️ using Flutter & Dart</sub>
  <br>
  <sub>© 2026 — Note App</sub>
</div>
