<div align="center">

<img src="app/src/main/res/drawable/ic_cyber_heist.jpg" alt="CYBER HEIST // BLACKOUT" width="100%" />

# CYBER HEIST // BLACKOUT

<strong>Enter the breach. Learn the defense. Survive the blackout.</strong>

<p>
  <img src="https://img.shields.io/badge/Android-Compose-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" />
  <img src="https://img.shields.io/badge/Kotlin-2.x-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" />
  <img src="https://img.shields.io/badge/Jetpack%20Compose-UI-4285F4?style=for-the-badge&logo=android&logoColor=white" alt="Jetpack Compose" />
  <img src="https://img.shields.io/github/stars/MrCheeku/Cyber-Heist-Blackout?style=for-the-badge&label=STARS" alt="GitHub stars" />
</p>

<p>
  <a href="https://github.com/MrCheeku"><img src="https://img.shields.io/badge/ENGINEERED%20BY-Mr.Cheeku-111827?style=for-the-badge&logo=github&logoColor=white" alt="Engineered by Mr.Cheeku" /></a>
</p>

</div>

---

## 🕶️ What is Cyber Heist // Blackout?

**Cyber Heist // Blackout** is an immersive Android cybersecurity game built with **Kotlin + Jetpack Compose**. It turns defensive-security concepts into an interactive cyber-operation: follow the story, solve technical puzzles, inspect simulated threats, strengthen defenses, and learn why the controls matter.

The project is designed as a **safe simulation**. The terminal, network, attack-box, credentials, packets, and target systems are fictional game systems rather than real-world infrastructure.

### ✨ Highlights

| Capability | What it does |
|---|---|
| **Cinematic Boot Sequence** | Drops the player into the operation with a cyberpunk terminal-style intro. |
| **Mission System** | Progress through story-driven missions with stateful objectives, scores, upgrades, and endings. |
| **Interactive Security Lab** | Explore hands-on simulations built around common security concepts. |
| **Network Maze** | Navigate a fictional network puzzle and make defensive decisions under pressure. |
| **Encryption Puzzles** | Solve encoding/crypto-inspired challenges to advance the story. |
| **Digital Forensics** | Investigate simulated evidence and piece together what happened. |
| **Threat Radar** | Track fictional live events and respond to changing security conditions. |
| **Security Audit** | Review personal-security concepts and defensive controls in a guided experience. |
| **TryHackMe-style Lab** | Practice inside a self-contained attack-box/target-browser simulation with no external target required. |
| **Cyber AI Chat** | Optional Gemini-powered in-game assistant for explanations and mission guidance. |
| **Leaderboards & Upgrades** | Replay, improve your score, and customize your cyber-operator progression. |
| **Save Game** | Persist player progress locally on-device. |

> **Safety:** This app is an educational simulation. Do not use its fictional workflows, examples, or commands against systems you do not own or have explicit permission to test.

---

## 🎮 Core Experience

```text
BOOT → INVESTIGATE → SOLVE → DEFEND → UPGRADE → RESCAN → SURVIVE
```

The game combines narrative progression with technical mini-games. Each system feeds the central `CyberGameViewModel`, which coordinates missions, player state, threats, lab interactions, save data, and optional AI assistance.

---

## 🧭 Project Architecture

```mermaid
flowchart TB
    A[🕶️ CYBER HEIST // BLACKOUT] --> B[📱 Compose UI]
    B --> C[🎮 CyberGameViewModel]
    C --> D[🧠 Game Models]
    C --> E[💾 SaveGameManager]
    C --> F[🛡️ Security Simulations]
    C --> G[⚡ CyberAudioEngine]
    C --> H[🤖 Gemini Chat]
    D --> I[Mission Data]
    D --> J[Security Concepts]
    D --> K[THM-style Labs]
    D --> L[Server / Encryption Puzzles]
    H --> M[Gemini API]
    
    classDef root fill:#7c3aed,stroke:#c4b5fd,color:#fff,stroke-width:3px;
    classDef ui fill:#2563eb,stroke:#93c5fd,color:#fff,stroke-width:2px;
    classDef core fill:#0891b2,stroke:#67e8f9,color:#fff,stroke-width:2px;
    classDef data fill:#059669,stroke:#6ee7b7,color:#fff,stroke-width:2px;
    classDef feature fill:#d97706,stroke:#fcd34d,color:#fff,stroke-width:2px;
    classDef external fill:#475569,stroke:#cbd5e1,color:#fff,stroke-width:2px;
    class A root;
    class B ui;
    class C core;
    class D,E,I,J,K,L data;
    class F,G,H feature;
    class M external;
```

### 📂 Project structure

```text
🕶️ Cyber-Heist-Blackout
│
├── 📱 app/
│   ├── src/main/java/com/example/cyberheist/
│   │   ├── audio/
│   │   │   └── CyberAudioEngine.kt
│   │   ├── data/
│   │   │   ├── SaveGameManager.kt
│   │   │   ├── GeminiApiService.kt
│   │   │   └── GeminiChatRepository.kt
│   │   ├── model/
│   │   │   ├── GameState.kt
│   │   │   ├── MissionData.kt
│   │   │   ├── SecurityConcepts.kt
│   │   │   ├── ServerPuzzleModels.kt
│   │   │   ├── TryHackMeModels.kt
│   │   │   └── GeminiChatModels.kt
│   │   ├── ui/
│   │   │   ├── components/
│   │   │   └── screens/
│   │   └── viewmodel/
│   │       └── CyberGameViewModel.kt
│   ├── src/test/
│   └── src/androidTest/
│
├── ⚙️ gradle/
├── 📄 .env.example
├── 📄 SECURITY.md
├── 📄 CONTRIBUTING.md
├── 📄 LICENSE
├── ⚙️ build.gradle.kts
├── ⚙️ gradle.properties
├── ⚙️ settings.gradle.kts
└── 📖 README.md
```

### 🔄 How the pieces connect

```text
📱 Screens + Components
          │
          ▼
🎮 CyberGameViewModel
   ├──► 🧠 Mission / puzzle data
   ├──► 🛡️ Security simulations
   ├──► 💾 SaveGameManager
   ├──► 🔊 Audio engine
   └──► 🤖 Optional Gemini assistant
```

The repository keeps gameplay orchestration, reusable UI, data models, persistence, audio, and network-facing AI code separated so contributors can work on one layer without hunting through the whole app.

---

## 🛡️ Security & Privacy

Cyber Heist // Blackout is built around **fictional game data**, not production credentials or real attack targets.

- Real API keys belong in local secrets only; `.env` is ignored by Git.
- Release signing values are read from environment variables rather than stored in the repository.
- Debug builds use Android's normal debug signing instead of a checked-in keystore.
- The repository excludes common secret-bearing files such as `.env`, `.jks`, `.keystore`, `.pem`, `.key`, and credential files.
- The in-game attack scenarios are simulations. No real target discovery or exploitation infrastructure is bundled.

See [`SECURITY.md`](SECURITY.md) for the repository's security policy and secret-handling guidance.

---

## 🤖 Optional Gemini Assistant

The game can use a Gemini API key for its optional AI chat experience.

### Local configuration

Create a local `.env` file from the example:

```bash
cp .env.example .env
```

Then set:

```text
GEMINI_API_KEY=your_real_key_here
```

Never commit `.env`, API keys, copied secrets, or exported credentials.

> The app remains usable without a real key for the core offline game experience; AI chat requires a valid local configuration.

---

## 🚀 Getting Started

### Requirements

- Android Studio with a recent stable Android toolchain
- JDK 11+
- Android SDK matching the project's configured compile/target SDK

### Open the project

1. Clone this repository.
2. Open it in Android Studio.
3. Let Gradle sync complete.
4. Create `.env` only when you want the Gemini-powered features.
5. Run the `app` configuration on an emulator or Android device.

### Build from the command line

```bash
./gradlew assembleDebug
```

### Run tests

```bash
./gradlew test
```

For Android instrumentation tests, use an emulator/device and run:

```bash
./gradlew connectedAndroidTest
```

---

## 🧪 Testing

The project includes JVM tests, Android instrumentation tests, Compose UI screenshot support, Robolectric, and Roborazzi-related test tooling.

Before opening a pull request:

```bash
./gradlew test
./gradlew assembleDebug
```

---

## 🗺️ Roadmap

- [x] Story-driven cyber operations
- [x] Compose-based cyberpunk interface
- [x] Mission progression and multiple endings
- [x] Interactive encryption / encoding puzzles
- [x] Network and forensics simulations
- [x] Security concepts and defensive labs
- [x] Local save system
- [x] Optional Gemini AI assistant
- [ ] Expanded mission packs
- [ ] More accessibility options
- [ ] Achievement / challenge system
- [ ] Expanded replay modifiers
- [ ] Release-ready Play Store assets

---

## 🌐 Official Links

<div align="center">

<a href="https://techwithcheeku.lovable.app/"><img src="https://img.shields.io/badge/Visit%20Tech%20with%20Cheeku-Website-7c3aed?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Tech with Cheeku website" /></a>
<a href="https://github.com/MrCheeku"><img src="https://img.shields.io/badge/GitHub-Mr.Cheeku-111827?style=for-the-badge&logo=github&logoColor=white" alt="Mr.Cheeku on GitHub" /></a>
<a href="https://discord.gg/GWJvzcxu"><img src="https://img.shields.io/badge/Join%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>

</div>

---

## 👨‍💻 Engineered By

<div align="center">

<a href="https://github.com/MrCheeku"><img src="https://avatars.githubusercontent.com/u/235286067?v=4" width="88" height="88" alt="Mr.Cheeku" /></a>

### **Mr.Cheeku**

<a href="https://github.com/MrCheeku"><img src="https://img.shields.io/badge/View%20Developer%20Profile-↗-111827?style=for-the-badge&logo=github&logoColor=white" alt="Developer profile" /></a>

<br /><br />

<a href="https://github.com/MrCheeku/Cyber-Heist-Blackout/issues">Report an issue</a>
&nbsp;•&nbsp;
<a href="https://github.com/MrCheeku/Cyber-Heist-Blackout">View source</a>

</div>
