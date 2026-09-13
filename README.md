# 🕷️ PHISING WRAITH

<p align="center">
  <img src="https://img.shields.io/badge/Phising%20Wraith-Security%20Simulation-00ff88?style=for-the-badge" alt="Phising Wraith">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS%20%7C%20Termux-111111?style=for-the-badge" alt="Platforms">
</p>

<p align="center">
  <b>🛡️ Interactive Phishing-Awareness & Security Simulation Framework</b><br>
  Built for authorized cybersecurity labs, demonstrations, education, and defensive research.
</p>

---

## 🕷️ PhisingWraith.py Logo

<p align="center">
  <img src="a_dark_cyberpunk_neon_hacker_styled_promotional.png" alt="PhisingWraith.py Logo" width="900">
</p>

<p align="center">
  <b>PhisingWraith.py</b><br>
  <i>Simulate • Educate • Stay Secure</i>
</p>

> Place `a_dark_cyberpunk_neon_hacker_styled_promotional.png` in the same repository directory as `README.md` for the logo to render on GitHub.

---


# 📌 Overview

**Phising Wraith** is a terminal-based phishing-awareness and simulation framework.

It provides an interactive workflow for creating **controlled security exercises** without requiring users to manually configure every component. The project includes terminal UI elements, template selection, dependency checks, local PHP hosting, optional tunnel support, environment detection, and safety/consent functionality.

The source currently contains:

- Interactive terminal menus
- Animated/banner-based presentation
- Multiple simulation templates
- Automatic dependency detection
- Termux-aware environment handling
- Local PHP server setup
- Local/LAN hosting information
- Optional `cloudflared` integration
- Configurable ports
- Connectivity/status checks
- Update checking
- Consent/disclaimer injection
- Process cleanup

---

# ✨ Main Features

## 🎨 1. Animated CLI Interface

Phising Wraith is designed to feel like a dedicated cybersecurity application rather than a collection of shell commands.

Recommended UI sequence:

```text
Boot
 ↓
Logo Animation
 ↓
Environment Scan
 ↓
Dependency Progress
 ↓
Safety Check
 ↓
Exercise Selection
 ↓
Server Initialization
 ↓
Live Lab Status
 ↓
Results
```

Suggested animation effects:

- Typewriter text
- Loading spinner
- Progress bar
- Matrix-style character stream
- Status check animation
- Template-selection transitions
- Server startup animation
- Success/failure indicators

---

# 🧩 2. Template Selection

The current source contains template-selection menus for multiple services, including:

- Facebook
- Instagram
- Google/Gmail
- Other templates included with the repository

These should be used **only as controlled simulation material**.

For an awareness exercise, participants should use synthetic/test information rather than real passwords, OTPs, recovery codes, or personal information.

---

# 🛠️ 3. Automatic Environment Setup

The application checks for required command-line utilities and prepares the local environment.

The source includes explicit handling for:

- Python
- PHP
- curl
- unzip
- Termux/proot
- `cloudflared`
- Several Linux package managers
- CPU architecture detection

---

# 🌍 Installation — All Supported Operating Systems

## 🪟 Windows

### Step 1 — Install Python

Install Python 3.x and make sure **Add Python to PATH** is enabled.

Verify:

```powershell
python --version
```

or:

```powershell
py --version
```

### Step 2 — Install PHP

Install PHP and verify:

```powershell
php --version
```

Make sure the PHP directory is available through your system `PATH`.

### Step 3 — Download the repository

```powershell
git clone <YOUR-REPOSITORY-URL>
cd Phising-Wraith
```

### Step 4 — Run

```powershell
python PhisingWraith.py
```

If your entry-point filename is different, replace `PhisingWraith.py` with the actual filename.

### Windows troubleshooting

Check:

```powershell
where python
where php
```

If either command returns nothing, install the missing dependency or add it to `PATH`.

---

# 🐧 Linux

## Debian / Ubuntu / Kali

Install the basic dependencies:

```bash
sudo apt update
sudo apt install python3 php curl unzip git -y
```

Verify:

```bash
python3 --version
php --version
curl --version
```

Clone:

```bash
git clone <YOUR-REPOSITORY-URL>
cd Phising-Wraith
```

Run:

```bash
python3 PhisingWraith.py
```

## Fedora

```bash
sudo dnf install python3 php curl unzip git -y
```

Then:

```bash
python3 PhisingWraith.py
```

## Arch Linux

```bash
sudo pacman -S python php curl unzip git
```

Then:

```bash
python3 PhisingWraith.py
```

---

# 🍎 macOS

Install Homebrew if it is not already installed.

Then install dependencies:

```bash
brew install python php curl unzip git
```

Verify:

```bash
python3 --version
php --version
```

Clone:

```bash
git clone <YOUR-REPOSITORY-URL>
cd Phising-Wraith
```

Run:

```bash
python3 PhisingWraith.py
```

---

# 📱 Termux / Android

Update packages:

```bash
pkg update && pkg upgrade -y
```

Install dependencies:

```bash
pkg install python php curl unzip git -y
```

Clone:

```bash
git clone <YOUR-REPOSITORY-URL>
cd Phising-Wraith
```

Run:

```bash
python3 PhisingWraith.py
```

The source already contains Termux-aware handling for environment preparation.

---

# 🔧 Installation Verification

Before starting an exercise, verify the basic environment:

```bash
python3 --version
php --version
curl --version
```

Then launch:

```bash
python3 PhisingWraith.py
```

A successful startup should progress approximately as follows:

```text
[✓] Python ................. OK
[✓] PHP .................... OK
[✓] curl ................... OK
[✓] Workspace .............. OK
[✓] Safety layer ........... READY
[✓] Simulation engine ...... READY

        PHISING WRAITH
             READY
```

---

# 🧪 Working Process

The recommended safe workflow is:

```text
┌──────────────────────┐
│ 1. Launch Application │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ 2. Environment Check │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ 3. Select Simulation │
│       Template       │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ 4. Consent / Safety  │
│        Gate          │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ 5. Start Local PHP   │
│       Server         │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ 6. Run Authorized    │
│       Exercise       │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ 7. Record Safe       │
│   Awareness Events   │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ 8. Show Results      │
└──────────────────────┘
```

---

# 🖥️ Local Laboratory Server

The project can prepare a selected simulation directory and start a PHP development server.

Conceptually:

```text
Phising Wraith
      │
      ├── Template
      │
      ├── Safety / Consent
      │
      └── PHP Server
             │
             ├── Localhost
             └── Authorized LAN Lab
```

The source also displays local/LAN hosting information after the server is prepared.

---

# 🔗 Optional Tunnel

The project includes optional `cloudflared` integration.

The source detects the machine architecture and prepares the corresponding tunnel binary.

Use a tunnel **only for an authorized laboratory that you control**.

For normal learning, localhost or an isolated LAN is preferable.

---

# ⚙️ Port Configuration

The application includes configurable port handling.

If a port is already occupied, choose another unused port.

Linux/macOS example:

```bash
ss -ltn
```

or:

```bash
lsof -i
```

Windows:

```powershell
netstat -ano
```

---

# 🛡️ Safety Architecture

A safe phishing-awareness simulator should follow:

```text
Participant
     ↓
Simulation Page
     ↓
Consent / Disclosure
     ↓
Synthetic Test Input
     ↓
Event / Awareness Result
     ↓
Report
```

It should **not** be designed around collecting real credentials.

Recommended telemetry:

```text
login_attempted = true
simulation_id   = LAB-001
template        = DEMO
timestamp       = exercise-time
```

Avoid storing:

```text
real_password
real_otp
recovery_code
session_cookie
private_token
```

---

# 🔐 Responsible Use

Phising Wraith is intended for:

- Cybersecurity education
- Phishing-awareness training
- Authorized penetration-testing laboratories
- Classroom demonstrations
- CTF-style controlled exercises
- Defensive security research

## ❌ Do not use it for

- Credential theft
- Account takeover
- Unauthorized access
- Real-world phishing
- Collection of real passwords or OTPs
- Unauthorized tracking
- Impersonating organizations against unsuspecting users

**Always obtain explicit authorization before running a security exercise.**

---

# 🧹 Cleanup

After a laboratory exercise:

1. Stop the local server.
2. Stop any optional tunnel.
3. Remove temporary simulation files.
4. Remove test participant data.
5. Review the exercise results.
6. Reset the laboratory environment.

A future hardened implementation should automate this cleanup.

---

# 📂 Suggested Project Structure

```text
Phising-Wraith/
│
├── PhisingWraith.py
├── README.md
├── LICENSE
│
├── .sites/
│   ├── facebook/
│   ├── instagram/
│   ├── google/
│   └── ...
│
├── .server/
│
├── auth/
│
├── www/
│
└── docs/
    └── demo.gif
```

Directory names may differ between project versions.

---

# 🏗️ Architecture

```text
                 ┌─────────────────────┐
                 │   PHISING WRAITH    │
                 │      CLI CORE       │
                 └──────────┬──────────┘
                            │
                 ┌──────────▼──────────┐
                 │ Environment Manager │
                 └──────────┬──────────┘
                            │
                 ┌──────────▼──────────┐
                 │ Exercise Templates  │
                 └──────────┬──────────┘
                            │
                 ┌──────────▼──────────┐
                 │ Safety / Consent    │
                 │       Layer         │
                 └──────────┬──────────┘
                            │
                 ┌──────────▼──────────┐
                 │   Local PHP Lab     │
                 │       Server        │
                 └──────────┬──────────┘
                            │
                   ┌────────┴────────┐
                   ▼                 ▼
              Local/LAN        Optional Tunnel
                   │                 │
                   └────────┬────────┘
                            ▼
                 ┌─────────────────────┐
                 │ Awareness Results  │
                 └─────────────────────┘
```

---

# 🎯 Roadmap

## v2.x

- [x] Interactive CLI
- [x] Animated terminal presentation
- [x] Template selection
- [x] Dependency checking
- [x] Local PHP server
- [x] Termux support
- [x] Optional tunnel integration
- [x] Consent/disclaimer functionality

## Future

- [ ] Fully synthetic credential simulator
- [ ] No-password telemetry architecture
- [ ] Interactive awareness dashboard
- [ ] Exercise statistics
- [ ] Campaign/session IDs
- [ ] Automatic cleanup
- [ ] Configuration file
- [ ] Stronger dependency verification
- [ ] Better Windows/macOS testing
- [ ] Automated unit tests
- [ ] Structured JSON reports

---

# 🐛 Troubleshooting

### `python3: command not found`

Install Python for your operating system and verify:

```bash
python3 --version
```

On Windows:

```powershell
python --version
```

### `php: command not found`

Install PHP and verify:

```bash
php --version
```

### Template not found

Confirm that the selected template exists in the project's template directory.

### Port already in use

Select another unused port.

### Tunnel unavailable

Run the exercise locally first. Tunneling is optional and should not be required for a basic laboratory.

### Permission error

On Linux/macOS, verify that the project directory is writable and that required executables have appropriate permissions.

---

# 👨‍💻 Author

**Sayed Eslamuddin**

**Engineered & Designed by Sayed Eslamuddin**

---

# ⭐ Project Vision

Phising Wraith aims to make phishing-awareness exercises:

> **Interactive • Educational • Controlled • Privacy-Aware • Easy to Operate**

The project focuses on helping learners understand how convincing phishing workflows can appear while keeping the exercise inside an authorized security laboratory.

---

# 📜 Disclaimer

This project is intended for **authorized cybersecurity education, research, and controlled security testing only**.

The user is responsible for obtaining permission before conducting any exercise.

**Never use real credentials, OTPs, recovery codes, session cookies, or other secrets during testing.**

---

<p align="center">
  <b>🛡️ Learn the attack. Understand the risk. Improve the defense.</b>
</p>
