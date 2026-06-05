# 🟢 Username Finder V23

<p align="center">
  <b>Premium Snoxy.dev Username Verification Dashboard</b><br>
  Trusted username checking • Clean proof system • Verified-only Discord logging
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Version-V23-brightgreen?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Platform-Windows-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Developer-Snoxy.dev-00ff66?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Logging-Verified_Only-success?style=for-the-badge" />
</p>

---

## 📌 Overview

**Username Finder V23** is a premium dark-green Snoxy.dev dashboard built for clean, structured, and trusted username verification.

The app is designed to manage username candidates, validate platform rules, import trusted proof data, maintain clean local caches, and send high-quality Discord logs only when a username is truly verified as available.

It does **not** treat generated usernames as real available names.  
A username is only marked as valid or taken when trusted proof exists.

---

## ✨ Key Features

- 🔍 **Single TrueCheck** for focused username validation
- 🌐 Platform structure for:
  - Discord
  - TikTok
  - Instagram
  - Telegram
  - Snapchat
- ✅ Clean truth-based result system
- 🧠 Smart local candidate generation
- 🧹 Duplicate, invalid, taken, and verified cache handling
- 📁 Trusted CSV proof import system
- 📊 Live dashboard with real-time counters
- 🖥️ Dark Snoxy.dev interface with green cyber-style design
- 📢 Verified-only Discord webhook logging
- 🛡️ No fake availability claims
- ⚙️ No admin rights required
- 🚀 Lightweight local Windows installation

---

## 🧠 Verification Logic

Username Finder V23 separates:

```text
Candidate Generation ≠ Real Verification
```

Generated usernames are only possible candidates.  
They are **not** automatically considered available.

A username becomes a trusted result only when it comes from one of these sources:

- manual proof,
- trusted CSV import,
- verified local database,
- official or allowed provider adapter.

This keeps results clean, reliable, and safe.

---

## ✅ Result Status System

| Status | Meaning |
|---|---|
| ✅ `VALID_VERIFIED` | The username is confirmed available by trusted proof |
| ❌ `TAKEN_VERIFIED` | The username is confirmed taken or unavailable |
| ⚠️ `INVALID_RULE` | The username does not match platform rules |
| ❔ `UNKNOWN_UNVERIFIED` | The format may be valid, but no trusted proof exists yet |

Only `VALID_VERIFIED` usernames are allowed to trigger Discord logs.

---

## 🖥️ Dashboard Sections

Username Finder V23 includes a clean and structured dashboard:

- 🟢 **Platforms**  
  Select which platforms should be included.

- 🔤 **Length + Characters**  
  Configure username length and character rules.

- 🔎 **Single TrueCheck**  
  Check one specific username with clear status output.

- 🌐 **Manual Browser Proof**  
  Open a selected profile page manually for proof-based review.

- 📊 **Results Table**  
  View structured username results with platform, status, source, latency, and score.

- 📁 **Valid Queue**  
  Manage verified available usernames.

- 🧹 **Taken / Invalid Cache**  
  Prevent repeated checks of known invalid or taken usernames.

- 📢 **Discord Logs**  
  Send clean alerts only for trusted verified available usernames.

---

## 📢 Discord Webhook Logging

Discord logging is designed to be clean, structured, and professional.

The app logs only usernames with this status:

```text
VALID_VERIFIED
```

It does **not** log:

```text
UNKNOWN_UNVERIFIED
INVALID_RULE
TAKEN_VERIFIED
LOCAL_CANDIDATE
PREDICTED_RESULT
```

This prevents fake hits, spam, and misleading alerts.

### Example Discord Log Content

```text
🟢 New Verified Username Found

Platform: Instagram
Username: example
Status: VALID_VERIFIED
Source: Trusted Import
Verification: Proof-Based
Time: 2026-06-05 19:30
```

---

## 🚀 Installation

### 1. Download

Download the latest ZIP release.

### 2. Extract

Extract the ZIP completely before running the setup.

### 3. Run Setup

Start the installer:

```bat
START_INSTALL.cmd
```

### 4. Install Location

The app installs locally to:

```text
%LocalAppData%\SnoxyDev\UsernameFinder
```

### 5. Start

After installation, the app opens automatically.

---

## ▶️ How to Use

1. Open **Username Finder V23**.
2. Select the platforms you want to work with.
3. Enter a username in **Single TrueCheck**.
4. Click **CHECK USERNAME**.
5. Review the result:
   - ✅ `VALID_VERIFIED`
   - ❌ `TAKEN_VERIFIED`
   - ⚠️ `INVALID_RULE`
   - ❔ `UNKNOWN_UNVERIFIED`
6. Import trusted proof data if needed.
7. Configure Discord webhook logging.
8. Verified available usernames can be logged automatically.

---

## 📁 Trusted Proof Import

The app supports trusted CSV imports for verified username data.

Example CSV format:

```csv
Platform,Username,Status,Source,LatencyMs,Score
Instagram,example,VALID_VERIFIED,Manual Proof,120,98
TikTok,testname,TAKEN_VERIFIED,Trusted Import,90,95
Discord,bad name,INVALID_RULE,Local Rule Check,0,0
```

Supported trusted statuses:

```text
VALID_VERIFIED
TAKEN_VERIFIED
INVALID_RULE
UNKNOWN_UNVERIFIED
```

---

## 🛡️ Safety Design

Username Finder V23 is built around safety and clean verification.

- No fake valid results
- No unsafe mass scraping
- No hidden downloads
- No admin rights required
- No SDK required
- No compiler required
- No misleading Discord alerts
- No generated username is treated as verified without proof

The app focuses on trusted verification, structured caching, local stability, and high-quality output.

---

## 🧩 Provider System

The app includes a provider-ready structure for future integrations.

A provider can be used only when it is official, allowed, and trusted.

Provider results should return clear proof-based statuses:

```text
VALID_VERIFIED
TAKEN_VERIFIED
INVALID_RULE
UNKNOWN_UNVERIFIED
```

This makes the system expandable without breaking the trusted verification model.

---

## 🧹 Cache System

Username Finder V23 keeps local cache files to avoid repeated work.

Cache categories include:

- checked usernames
- invalid usernames
- taken usernames
- verified available usernames
- trusted imported proof data

This helps keep the app faster, cleaner, and more stable.

---

## 🧪 Debugging

If the app does not start correctly, use the debug launcher:

```text
%LocalAppData%\SnoxyDev\UsernameFinder\Start_UsernameFinder_DEBUG.cmd
```

Useful log files:

```text
%LocalAppData%\SnoxyDev\UsernameFinder\install.log
%LocalAppData%\SnoxyDev\UsernameFinder\app.log
%LocalAppData%\SnoxyDev\UsernameFinder\crash.log
%LocalAppData%\SnoxyDev\UsernameFinder\webhook_results.log
%LocalAppData%\SnoxyDev\UsernameFinder\provider_gateway.log
```

---

## 📦 Requirements

Username Finder V23 is designed for Windows.

Required components are checked by the setup:

- Windows
- `mshta.exe`
- Windows PowerShell 5.1
- Local user write access to `%LocalAppData%`

No admin rights are required.

---

## 🔐 Privacy

The app runs locally and stores its data inside the user profile.

Default data location:

```text
%LocalAppData%\SnoxyDev\UsernameFinder
```

Webhook settings and local cache files stay on the local machine.

---

## 👨‍💻 Developer

Developed by **Snoxy.dev**

```text
Project: Username Finder
Version: V23
Developer: Snoxy.dev
Focus: Trusted username verification
Design: Dark green enterprise dashboard
```

---

## ⚠️ Disclaimer

Username Finder V23 is designed for trusted verification workflows.  
It does not guarantee username availability unless a result is confirmed by trusted proof, verified import, manual proof, or an allowed official provider.

Generated usernames are candidates only and should not be treated as confirmed availability.

---

<p align="center">
  <b>Username Finder V23</b><br>
  Clean checks • Trusted proof • Verified-only logs • Snoxy.dev
</p>
