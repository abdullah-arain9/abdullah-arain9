<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=1000&color=02569B&center=true&vCenter=true&width=700&lines=Hi+%F0%9F%91%8B+I'm+Abdullah+Arain;Full+Stack+Flutter+Developer;GSoC+2026+Applicant+%7C+Dart+Org;Open+Source+Contributor+%F0%9F%9A%80" alt="Typing SVG" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/abdullah-arain9)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:arainabdullah225@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/abdullah-arain9)

</div>

---

## 👨‍💻 About Me

<img align="right" alt="Coding" width="340" src="https://user-images.githubusercontent.com/74038190/229223263-cf2e4b07-2615-4f87-9c38-e37600f8381a.gif"/>

```dart
class Abdullah extends FlutterDeveloper {

  final String name     = "Abdullah Arain";
  final String role     = "Full Stack Flutter Developer";
  final String location = "Karachi, Pakistan 🇵🇰";

  final List<String> currentFocus = [
    "GSoC 2026 — Dart DevTools",
    "WebSocket/gRPC Network Profiling",
    "Mobile POS Systems",
  ];

  final List<String> openTo = [
    "Remote Jobs",
    "Freelancing",
    "Open Source",
    "Full-Time",
  ];

  String get funFact =>
    "I digitize local shops one app at a time 🏪";
}
```

<br clear="right"/>

I'm a Flutter developer from Karachi building production-ready mobile apps with clean architecture. Currently applying for **Google Summer of Code 2026** with the Dart organization — working on WebSocket/gRPC support for Flutter DevTools.

---

## 🛠️ Tech Stack

<div align="center">

**Mobile & Language**

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-0175C2?style=for-the-badge&logo=dart&logoColor=white)

**Backend & Database**

![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Firestore](https://img.shields.io/badge/Firestore-FF6F00?style=for-the-badge&logo=firebase&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Hive](https://img.shields.io/badge/Hive-FFB300?style=for-the-badge&logo=hive&logoColor=black)

**Architecture & Tools**

![Clean Architecture](https://img.shields.io/badge/Clean%20Architecture-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![REST API](https://img.shields.io/badge/REST%20API-FF5733?style=for-the-badge&logo=postman&logoColor=white)
![Provider](https://img.shields.io/badge/Provider-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Android Studio](https://img.shields.io/badge/Android%20Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)

</div>

---

## 🌐 GSoC 2026 — Open Source Work

### WebSocket DevTools Profiler
> **Organization:** Dart &nbsp;|&nbsp; **Project:** Add WebSocket/gRPC Support to Flutter DevTools Network Panel

Currently building a working instrumentation layer that surfaces **WebSocket traffic inside Flutter DevTools** — using the same `dart:developer` Timeline mechanism that HTTP profiling uses today.

[![Repo](https://img.shields.io/badge/GitHub-websocket--devtools--profiler-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdullah-arain9/websocket-devtools-profiler)

**What it does:**

```
ID   TIME           DIR    TYPE   BYTES   ELAPSED     PREVIEW
──   ─────────────  ─────  ────   ─────   ─────────   ───────────────────────
1    14:06:41.786   sent   text   20B     +22274ms    hello GSOC community
2    14:06:42.196   recv   text   20B     +22684ms    hello GSOC community
3    14:06:53.829   sent   text   17B     +34317ms    its Abdullah Here
4    14:06:54.090   recv   text   17B     +34578ms    its Abdullah Here

Summary → Connections: 1  |  Sent: 67B  |  Received: 67B
```

**Technical decisions:**
- `ProfileableWebSocket` implements `dart:io` WebSocket — zero breaking changes, drop-in replacement
- Events posted via `dart:developer.Timeline.instantSync()` — same pipeline as HTTP profiling
- `WebSocketProfiler` registry handles multiple simultaneous connections
- 9 unit tests, all passing — no network required (MockWebSocket)

**Next steps (in progress):**
- [ ] gRPC channel instrumentation layer
- [ ] DevTools panel UI — message timeline & byte counters
- [ ] Stream diffing for large binary frames

---

## 🚀 Featured Projects

### 📱 Developer Invoice Tracker — Mobile POS & Shop Management

A production-level mobile POS system built for local shopkeepers to fully digitize their business — no expensive desktop software or hardware needed.

[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)](https://flutter.dev)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white)](https://dart.dev)
[![Provider](https://img.shields.io/badge/Provider-02569B?style=flat-square&logo=flutter&logoColor=white)](https://pub.dev/packages/provider)

| Feature | Description |
|---|---|
| 🧾 Invoice Generation | Auto-generated branded invoices per sale |
| 🖨️ Thermal Printing | Bluetooth thermal printer integration |
| 📦 Product Management | Full inventory tracking & stock alerts |
| 📊 Sales Analytics | Daily sales history & summary reports |
| 🏪 Shop Dashboard | Single-app business control center |

**Architecture:**
```
lib/
├── core/          → theme, constants, error handling
├── data/          → repositories, models, Firebase & local sources
├── domain/        → business logic, use cases
└── presentation/  → screens, widgets, providers
```

---

### 💬 Real-Time Chat App *(in progress)*

End-to-end real-time messaging with Firebase backend, Google sign-in, image sharing, and push notifications.

[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)](https://flutter.dev)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com)
[![Firestore](https://img.shields.io/badge/Firestore-FF6F00?style=flat-square&logo=firebase&logoColor=white)](https://firebase.google.com)

---

### 🛒 E-Commerce App *(in progress)*

Full shopping experience with REST API backend, cart management, order tracking, and secure auth.

[![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)](https://flutter.dev)
[![REST API](https://img.shields.io/badge/REST%20API-FF5733?style=flat-square&logo=postman&logoColor=white)](https://pub.dev/packages/http)
[![Provider](https://img.shields.io/badge/Provider-02569B?style=flat-square&logo=flutter&logoColor=white)](https://pub.dev/packages/provider)

---

## 📊 GitHub Stats

<div align="center">

<img width="49%" src="https://github-readme-stats.vercel.app/api?username=abdullah-arain9&show_icons=true&theme=dark&hide_border=true&count_private=true&include_all_commits=true" />
<img width="49%" src="https://github-readme-streak-stats.herokuapp.com/?user=abdullah-arain9&theme=dark&hide_border=true" />

<img width="40%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=abdullah-arain9&layout=compact&theme=dark&hide_border=true&langs_count=6" />

</div>

---

## 📬 Connect

I'm open to collaborating on Flutter projects, open source, freelance, or remote full-time roles.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/abdullah-arain9)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:arainabdullah225@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abdullah-arain9)

---

<div align="center">

*"I build mobile experiences that are fast, scalable, and production-ready — and contribute to open source to make developer tools better for everyone."*

</div>
