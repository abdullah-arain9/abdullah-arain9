# Hi, I'm Abdullah Arain 👋

![Profile Views](https://komarev.com/ghpvc/?username=abdullah-arain9&label=Profile%20Views&color=0e75b6&style=flat-square)

💻 Flutter Developer | GSoC 2026 Applicant | Dart Open Source Contributor  
Building scalable, production-ready mobile applications with clean architecture and real-world impact.

---

## About Me

I am **Abdullah Arain**, a **Full Stack Flutter Developer** from **Karachi, Pakistan** with hands-on experience building production-level mobile applications using **Flutter and Dart**.

Currently applying for **Google Summer of Code 2026** with the **Dart organization** — working on adding **WebSocket/gRPC support** to the Flutter DevTools Network Panel.

Alongside app development, I have shipped real-world business solutions including a **Mobile POS and Shop Management System** used by local shopkeepers to digitize their operations.

---

## Tech Stack

- **Mobile:** Flutter, Dart, Responsive UI, Material Design, Custom Widgets
- **State Management:** Provider, ChangeNotifier, App State Management
- **Backend & Services:** Firebase Auth, Cloud Firestore, Firebase Storage, Realtime Database
- **API:** REST API Integration, JSON Parsing, HTTP Requests
- **Database:** Firestore, Hive, SQLite, Local Storage
- **Architecture:** Clean Architecture, MVC, MVVM, Scalable Folder Structure
- **Tools:** Git, GitHub, Android Studio, VS Code, Postman, Firebase Console

---

## GSoC 2026 — Open Source Contribution

### WebSocket DevTools Profiler
> **Organization:** Dart | **Project:** Add WebSocket/gRPC Support to Flutter DevTools Network Panel

Built a working instrumentation layer demonstrating how WebSocket traffic can be surfaced in Flutter DevTools — using the same `dart:developer` Timeline mechanism that HTTP profiling uses today.

[![GitHub](https://img.shields.io/badge/GitHub-websocket--devtools--profiler-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdullah-arain9/websocket-devtools-profiler)
```
ID   TIME           DIR    TYPE   BYTES   ELAPSED     PREVIEW
1    14:06:41.786   sent   text   20B     +22274ms    hello GSOC community
2    14:06:42.196   recv   text   20B     +22684ms    hello GSOC community
3    14:06:53.829   sent   text   17B     +34317ms    its Abdullah Here
4    14:06:54.090   recv   text   17B     +34578ms    its Abdullah Here

Summary: Connections: 1 | Sent: 67B | Received: 67B
```

**Key decisions:**
- `ProfileableWebSocket` implements `dart:io` WebSocket — drop-in replacement
- Events posted via `dart:developer.Timeline.instantSync()` — same as HTTP profiling
- `WebSocketProfiler` registry manages multiple simultaneous connections
- 9 unit tests passing — no network required (MockWebSocket)

---

## Featured Projects

### Developer Invoice Tracker — Mobile POS & Shop Management App

A real-world mobile application for local shopkeepers to digitize their business operations through a single mobile device.

**Key Features:**
- Product & Daily Sales Management
- Invoice Generation & POS Bill Printing
- Sales History Tracking
- Thermal Printer Integration
- Shop Management System

[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)](https://flutter.dev)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)](https://dart.dev)

---

## GitHub Stats

![Abdullah's GitHub Stats](https://github-readme-stats.vercel.app/api?username=abdullah-arain9&show_icons=true&theme=dark&hide_border=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=abdullah-arain9&layout=compact&theme=dark&hide_border=true)

---

## Connect With Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/abdullah-arain9)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:arainabdullah225@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdullah-arain9)

---

> "I build mobile experiences that are fast, scalable, and production-ready — and contribute to open source to make developer tools better for everyone."
