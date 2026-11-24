<p align="center">
  <img src="./nazaru-banner.png" alt="NAZARU — The Digital Guardian" width="100%">
</p>


## Origin of the Name – NAZARU
The name **NAZARU** is inspired by the ancient Akkadian words Naṣāru (to guard, protect, and preserve) and Nāṣiru (guardian or protector).

Inspired by these meanings, NAZARU represents the mission of the tool: to identify security weaknesses, protect Linux systems, and help preserve their integrity.


---

## 📌 Project Description

**NAZARU** is a Bash-based Linux security auditing tool that evaluates a system against a collection of 40 security and hardening checks.

It examines important areas of Linux system security, including SSH configuration, user accounts, authentication policies, network services, firewall status, file permissions, system services, logging, and security monitoring.

NAZARU collects system information, evaluates security conditions, and classifies its findings using clear status levels to help administrators understand the security posture of their Linux systems.

The tool is designed to run locally without requiring a centralized security platform or external service.

---

## 👥 Who Is NAZARU For?

| Audience | Purpose |
|---|---|
| 🔐 Security Engineers | Identify Linux security weaknesses and hardening gaps |
| 🧪 Penetration Testers | Perform initial security configuration assessments |
| 🖥️ Linux System Administrators | Review server configurations and security settings |
| 🛡️ Blue Team Members | Support host security assessments and defensive reviews |
| 🏢 IT Security Teams | Perform repeatable Linux security checks |
| 🎓 Security Students | Learn Linux hardening concepts and security auditing |

---

## ✨ Key Advantages

- **🔍 40 Security Checks** — Evaluates 40 different areas of Linux system security.
- **⚡ Lightweight** — Implemented in Bash without requiring a large application stack.
- **🔒 Local Execution** — Performs assessments directly on the target Linux system.
- **📊 Clear Results** — Uses structured security statuses to make findings easy to understand.
- **📝 Report Generation** — Supports saving scan results to a report file.
- **🎨 Readable Output** — Uses colored terminal output and a custom command-line banner.
- **🧩 Broad Coverage** — Examines authentication, SSH, network exposure, permissions, logging, monitoring, and more.
- **🚫 Read-Only Assessment** — Designed to inspect system security without intentionally modifying system settings.

---

## 🔎 Security Assessment Coverage

NAZARU currently includes 40 security checks organized around the following areas:

| Category | Checks |
|---|---|
| 🔑 SSH Security | Root login, password authentication, management access restrictions |
| 👤 Account Security | Root account status, UID 0 accounts, empty passwords, administrative groups |
| 🔐 Authentication | Password aging, PAM lockout, MFA indicators |
| 🌐 Network Security | Listening sockets, Telnet, FTP, Samba, SNMP |
| 🔥 Firewall & Boot Security | Firewall status, reboot indicator, Secure Boot, GRUB protection |
| 🛡️ System Hardening | SELinux, AppArmor, automatic security updates |
| 📁 File System Security | Critical file permissions, SUID/SGID, world-writable files, capabilities |
| ⚙️ Persistence & Services | Cron access, startup scripts, enabled systemd services, cron persistence |
| 📋 Logging & Monitoring | Authentication logs, remote logging, privilege-change logging, EDR indicators |
| 💾 Integrity & Recovery | File integrity monitoring, backups, immutability indicators, restore-test evidence |

---

## 🚦 Result Classification

NAZARU uses six status levels to classify assessment results:

| Status | Meaning |
|---|---|
| 🟢 **PASS** | The check meets its defined security condition |
| 🟡 **WARN** | A potential security weakness or hardening gap was identified |
| 🔴 **FAIL** | A security condition was found to be non-compliant |
| 🔵 **INFO** | Informational result or inventory data |
| ⚪ **UNKNOWN** | The condition could not be reliably determined |
| ❗ **ERROR** | The check encountered an execution or inspection error |

> **Note:** `INFO` and `UNKNOWN` do not automatically indicate a security vulnerability. They may represent inventory information or conditions that cannot be verified locally.

---

## 🚀 How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/M0G3H/NAZARU.git
```

### 2. Enter the Project Directory

```bash
cd NAZARU
```

### 3. Make the Script Executable

```bash
chmod +x Nazaru
```

### 4. Run a Security Assessment

```bash
./Nazaru
```

Alternatively:

```bash
bash Nazaru
```

### 5. Save the Assessment Report

Provide a report filename as an argument:

```bash
./Nazaru nazaru_report.txt
```

The results will be displayed in the terminal and saved to the specified report file.

### 6. Run with Elevated Privileges (Optional)

```bash
sudo ./Nazaru
```

Running with elevated privileges can improve visibility into protected files, system configurations, and security settings. Use it when a more complete assessment is required.

---

## ⚠️ Important Notes

- NAZARU is intended for Linux systems.
- Some checks depend on available system utilities and distribution-specific configuration files.
- Running without root privileges may limit access to certain protected resources.
- `UNKNOWN` means that a condition could not be reliably verified; it should not be interpreted as secure.
- Always review findings before making system configuration changes.
- Use NAZARU only in systems you own or are authorized to assess.

---


<p align="center">
  **🛡️ NAZARU — See the Weakness. Strengthen the System.**
</p>
