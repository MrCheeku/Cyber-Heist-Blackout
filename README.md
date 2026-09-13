<div align="center">

<img src="assets/header.svg" alt="Cyber Heist — Blackout cybersecurity simulation" width="100%" />

<p>
  <a href="https://github.com/MrCheeku/Cyber-Heist-Blackout"><img src="https://img.shields.io/github/stars/MrCheeku/Cyber-Heist-Blackout?style=for-the-badge&label=STARS&cacheSeconds=60" alt="GitHub stars" /></a>
  <a href="https://github.com/MrCheeku/Cyber-Heist-Blackout"><img src="https://img.shields.io/github/last-commit/MrCheeku/Cyber-Heist-Blackout?style=for-the-badge&label=UPDATED" alt="Last commit" /></a>
  <a href="https://img.shields.io/github/repo-size/MrCheeku/Cyber-Heist-Blackout"><img src="https://img.shields.io/github/repo-size/MrCheeku/Cyber-Heist-Blackout?style=for-the-badge&label=SIZE" alt="Repository size" /></a>
</p>

<p><strong>Story-driven cyber operations • Security puzzles • Defensive learning • Android</strong></p>

<a href="https://github.com/MrCheeku"><img src="https://img.shields.io/badge/ENGINEERED%20BY-Mr.Cheeku-111827?style=for-the-badge&logo=github&logoColor=white" alt="Engineered by Mr.Cheeku" /></a>

</div>

---

## 🕶️ What is Cyber Heist // Blackout?

**Cyber Heist // Blackout** is an Android cybersecurity game that turns defensive-security concepts into a cinematic, interactive operation. Built with **Kotlin + Jetpack Compose**, it combines missions, simulated attacks, encryption puzzles, digital forensics, network challenges, security audits, upgrades, and an optional Gemini-powered assistant.

The world inside the app is a **self-contained simulation**. Targets, credentials, flags, packets, terminals, and attack-boxes are fictional game data.

### ✨ Highlights

| Capability | What it does |
|---|---|
| **Mission Campaign** | Story-driven operations with objectives, scores, upgrades, and multiple endings. |
| **Cyberpunk Interface** | Boot sequence, terminal UI, threat panels, animated backgrounds, audio, and themed Compose components. |
| **Interactive Security Lab** | Guided simulations and hands-on security mini-games. |
| **Network Maze** | Solve a fictional network-navigation challenge under pressure. |
| **Encryption Puzzles** | Encoding and cryptography-inspired challenges. |
| **Digital Forensics** | Inspect simulated evidence and reconstruct incidents. |
| **Threat Radar** | Respond to fictional real-time threat events. |
| **Personal Security Audit** | Review practical defensive-security habits and controls. |
| **TryHackMe-style Rooms** | Self-contained simulated rooms with no real targets. |
| **Gemini Cyber Assistant** | Optional AI chat for explanations, hints, and mission guidance. |
| **Progression System** | Leaderboards, upgrades, save data, replayability, and multiple outcomes. |

> ⚠️ **Safety rule:** use the project only as a simulation and educational tool. Never apply its workflows to systems you do not own or have explicit permission to test.

---

## ✨ Core Experience

```text
BOOT → INVESTIGATE → SOLVE → DEFEND → UPGRADE → RESCAN → SURVIVE
```

A central `CyberGameViewModel` coordinates player state, missions, simulated threats, puzzle interactions, persistence, audio, and optional AI assistance.

## 🎬 Cyber Operation Preview

<div align="center">

<img src="app/src/main/res/drawable/ic_cyber_heist.jpg" alt="Cyber Heist Blackout visual" width="900" />

> 🎥 **Visual preview:** the project includes its own cyberpunk artwork and themed Android UI. The complete experience contains missions, labs, terminal gameplay, forensics, encryption, threat radar, and simulated TryHackMe-style rooms.

</div>

---

## 🧰 Tech Stack

<div align="center">

### Android & UI
<img src="https://skillicons.dev/icons?i=android,kotlin,gradle" alt="Android, Kotlin, Gradle" />

### Architecture
<img src="https://img.shields.io/badge/Jetpack%20Compose-UI-4285F4?style=flat-square&logo=android&logoColor=white" alt="Jetpack Compose" />
<img src="https://img.shields.io/badge/ViewModel-Game%20State-0891b2?style=flat-square" alt="Android ViewModel" />
<img src="https://img.shields.io/badge/DataStore-Local%20Save-059669?style=flat-square" alt="DataStore" />
<img src="https://img.shields.io/badge/Retrofit-API%20Layer-48B983?style=flat-square" alt="Retrofit" />

### Security & AI
<img src="https://img.shields.io/badge/Cybersecurity-Simulation-DC2626?style=flat-square" alt="Cybersecurity simulation" />
<img src="https://img.shields.io/badge/Gemini-Optional%20AI-7c3aed?style=flat-square" alt="Gemini optional AI" />
<img src="https://img.shields.io/badge/Secrets-Environment%20Only-111827?style=flat-square" alt="Environment-only secrets" />

</div>

---

## 🧭 Project Structure

> 🎨 **Interactive Mermaid architecture:** compact, color-coded, and organized like the author's other repositories.

```mermaid
flowchart TB
    A[🕶️ Cyber Heist // Blackout] --> B[📱 Compose UI]
    B --> C[🎮 CyberGameViewModel]
    C --> D[🧠 Game & Mission Models]
    C --> E[🛡️ Security Simulations]
    C --> F[💾 SaveGameManager]
    C --> G[🔊 CyberAudioEngine]
    C --> H[🤖 Gemini Assistant]
    D --> I[🧩 Puzzle Data]
    D --> J[🧪 TryHackMe-style Rooms]
    E --> K[🔎 Forensics / Audit / Threat Radar]
    H --> L[☁️ Gemini API]

    classDef root fill:#7c3aed,stroke:#c4b5fd,color:#ffffff,stroke-width:3px;
    classDef ui fill:#2563eb,stroke:#93c5fd,color:#ffffff,stroke-width:2px;
    classDef core fill:#0891b2,stroke:#67e8f9,color:#ffffff,stroke-width:2px;
    classDef data fill:#059669,stroke:#6ee7b7,color:#ffffff,stroke-width:2px;
    classDef feature fill:#d97706,stroke:#fcd34d,color:#ffffff,stroke-width:2px;
    classDef external fill:#475569,stroke:#cbd5e1,color:#ffffff,stroke-width:2px;
    class A root;
    class B ui;
    class C core;
    class D,F,I,J data;
    class E,G,K feature;
    class H,L external;
```

### 📱 Mobile-friendly note

This is **real Mermaid source—not a screenshot**. GitHub controls Mermaid rendering in each client.

<details>
<summary>📂 View Project Structure as Text</summary>

```text
🕶️ Cyber-Heist-Blackout
│
├── 📱 app/
│   ├── 🧩 src/main/java/com/example/
│   │   ├── cyberheist/
│   │   │   ├── audio/
│   │   │   ├── data/
│   │   │   ├── model/
│   │   │   ├── ui/
│   │   │   │   ├── components/
│   │   │   │   └── screens/
│   │   │   └── viewmodel/
│   │   └── ui/theme/
│   ├── 🧪 src/test/
│   ├── 🧪 src/androidTest/
│   └── ⚙️ build.gradle.kts
│
├── 🎨 assets/
│   ├── header.svg
│   └── footer.svg
├── 🔑 .env.example
├── 🛡️ SECURITY.md
├── 🤝 CONTRIBUTING.md
├── 📄 LICENSE
├── 📋 metadata.json
├── ⚙️ build.gradle.kts
├── ⚙️ gradle.properties
├── 📦 gradle/libs.versions.toml
└── ⚙️ settings.gradle.kts
```

</details>

### 🔄 How the pieces connect

```text
📱 Compose Screens + Components
             │
             ▼
      🎮 Game ViewModel
       │    │    │    │
       │    │    │    └────► 🤖 Optional Gemini Assistant
       │    │    │
       │    │    └─────────► 🔊 Audio Engine
       │    │
       │    └──────────────► 💾 Local Save Data
       │
       └───────────────────► 🧠 Missions + Security Simulations
```

The repository separates UI, game orchestration, models, persistence, audio, simulations, and AI integration so contributors can locate each responsibility quickly.

---

## 🛡️ Security Design

- No real private keys or production credentials are required by the game.
- Gemini configuration is local-only through `GEMINI_API_KEY`.
- Release signing values are supplied through environment variables.
- Common secret-bearing files are ignored by Git.
- Simulated private-key content in educational rooms is redacted rather than storing usable key material.
- TryHackMe-style rooms are self-contained game simulations.

See [`SECURITY.md`](SECURITY.md) for the repository security policy.

---

## 🚀 Getting Started

### Requirements

- Android Studio with a recent stable Android/Gradle toolchain
- JDK 11+
- Android SDK matching the configured compile/target SDK

### Open in Android Studio

1. Clone the repository.
2. Open it in Android Studio.
3. Sync Gradle.
4. Run the `app` configuration on an emulator or Android device.

### Configure optional Gemini AI

Create a local `.env` from `.env.example` and set:

```text
GEMINI_API_KEY=your_real_key_here
```

> Never commit `.env`, API keys, keystores, passwords, or exported credentials.

---

## 🧪 Testing

The project includes JVM tests, Android instrumentation tests, Compose UI testing support, Robolectric, and Roborazzi screenshot tooling.

```bash
gradle test
gradle assembleDebug
gradle connectedAndroidTest
```

> The repository does not currently include the Gradle wrapper scripts (`gradlew` / `gradlew.bat`). You can run these tasks from Android Studio or from a system Gradle installation.

---

## ⚠️ Demo / Simulation Scope

Cyber Heist // Blackout is an educational game, not a production penetration-testing platform. Simulated terminals, flags, network addresses, attack-boxes, credentials, and vulnerabilities exist to support gameplay and learning.

---

## 🗺️ Roadmap

- [x] Story-driven cyber operations
- [x] Cyberpunk Jetpack Compose interface
- [x] Mission progression and multiple endings
- [x] Encryption / encoding puzzles
- [x] Network and forensics simulations
- [x] Security concepts and defensive labs
- [x] Local save system
- [x] Optional Gemini AI assistant
- [x] TryHackMe-style self-contained rooms
- [ ] Expanded mission packs
- [ ] More accessibility options
- [ ] Achievement / challenge system
- [ ] Expanded replay modifiers
- [ ] Release-ready Play Store assets

---

## 🌐 Official Links

<div align="center">

<p>
  <a href="https://techwithcheeku.lovable.app/"><img src="https://img.shields.io/badge/🌐%20Tech%20with%20Cheeku-Website-7c3aed?style=for-the-badge" alt="Visit Tech with Cheeku website" /></a>
</p>

<p>
  <a href="https://whatsapp.com/channel/0029Vb9OpwgD8SDvISwrn73Y"><img src="https://img.shields.io/badge/💬%20WhatsApp-Join%20the%20Channel-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="Join the Tech with Cheeku WhatsApp channel" /></a>
</p>

<p>
  <a href="https://discord.gg/GWJvzcxu"><img src="https://img.shields.io/badge/👾%20Discord-Join%20the%20Community-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join the Tech with Cheeku Discord community" /></a>
</p>

<sub>Official community and project links for Tech with Cheeku.</sub>

</div>

---

## 👨‍💻 Engineered By

<div align="center">

<a href="https://github.com/MrCheeku"><img src="https://avatars.githubusercontent.com/u/235286067?v=4" width="88" height="88" alt="Mr.Cheeku GitHub avatar" /></a>

### **Mr.Cheeku**

<a href="https://github.com/MrCheeku"><img src="https://img.shields.io/badge/Visit%20Developer%20Profile-↗-111827?style=for-the-badge&logo=github&logoColor=white" alt="Developer profile" /></a>

</div>

---

<div align="center">

<a href="https://github.com/MrCheeku/Cyber-Heist-Blackout/issues">Report an issue</a>
&nbsp;•&nbsp;
<a href="https://github.com/MrCheeku/Cyber-Heist-Blackout">View source</a>
&nbsp;•&nbsp;
<a href="https://github.com/MrCheeku">Developer profile</a>

<br /><br />

<img src="assets/footer.svg" alt="Cyber Heist Blackout footer" width="100%" />

</div>
