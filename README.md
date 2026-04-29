<div align="center">

# :skull: Reverse Shell Generator

[![Stars](https://img.shields.io/github/stars/geevarghesekthomas84-sys/reverse-shell-generator?style=for-the-badge&color=00ff41&logo=github)](https://github.com/geevarghesekthomas84-sys/reverse-shell-generator/stargazers)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Live_Demo-Click_Here-ff0040?style=for-the-badge&logo=github)](https://geevarghesekthomas84-sys.github.io/reverse-shell-generator/)

**A sleek, dark-themed web-based reverse shell payload generator for penetration testers and red teamers.**

One-click copy. Zero install. Works offline. No dependencies.

</div>

---

## :camera_flash: Screenshot

<p align="center">
  <img src="screenshot.png" alt="Reverse Shell Generator Screenshot" width="90%"/>
</p>

---

## :sparkles: Features

- :zap: **25+ Reverse Shell Payloads** — Bash, Netcat, Python, PHP, PowerShell, Perl, Ruby, Socat
- :art: **Dark Hacker UI** — Matrix-inspired design with syntax highlighting
- :clipboard: **One-Click Copy** — Click any payload to instantly copy to clipboard
- :arrows_counterclockwise: **Dynamic Generation** — Change IP/Port and all payloads update in real-time
- :lock: **Multiple Shell Types** — `/bin/sh`, `/bin/bash`, `/bin/zsh`, `cmd.exe`, `powershell`
- :shield: **Encoding Support** — None, Base64, URL encoding
- :iphone: **Responsive** — Works on desktop, tablet, and mobile
- :globe_with_meridians: **Zero Dependencies** — Single HTML file, no frameworks, no build step
- :airplane: **Works Offline** — Download and use without internet

---

## :rocket: Quick Start

### Option 1: Use Online (GitHub Pages)
Visit the live demo: [https://geevarghesekthomas84-sys.github.io/reverse-shell-generator/](https://geevarghesekthomas84-sys.github.io/reverse-shell-generator/)

### Option 2: Run Locally
```bash
# Clone the repo
git clone https://github.com/geevarghesekthomas84-sys/reverse-shell-generator.git

# Open in browser
open index.html
# or
python3 -m http.server 8080
```

### Option 3: Download Single File
Just download `index.html` — it's completely self-contained.

---

## :crossed_swords: Supported Payloads

| Language | Variants | Type |
|----------|----------|------|
| **Bash** | `-i`, Read Line, 196, UDP | TCP/UDP |
| **Netcat** | `-e`, `-c`, FIFO, Ncat SSL | TCP/SSL |
| **Python** | Short, PTY, Spawn | TCP |
| **PHP** | exec, proc_open, popen | WEB |
| **PowerShell** | #1, #2, Base64 | WIN |
| **Perl** | Standard, no-sh | TCP |
| **Ruby** | Standard, no-sh | TCP |
| **Socat** | TTY, Listener | TCP |
| **Listeners** | nc, rlwrap, pwncat, msfconsole | -- |
| **Shell Upgrade** | Python PTY, script | PTY |

---

## :keyboard: Usage

1. Enter your **listener IP** and **port**
2. Select your preferred **shell type** (`/bin/bash`, `cmd.exe`, etc.)
3. Choose **encoding** (None, Base64, URL)
4. Click **Copy** on any payload
5. Paste into your target

### Setting Up a Listener
```bash
# Basic netcat listener
nc -lvnp 4444

# With readline support
rlwrap nc -lvnp 4444

# Metasploit
msfconsole -q -x "use exploit/multi/handler; set PAYLOAD generic/shell_reverse_tcp; set LHOST 10.10.14.1; set LPORT 4444; run"
```

### Upgrading to Interactive Shell
```bash
# On target:
python3 -c 'import pty;pty.spawn("/bin/bash")'
# Press Ctrl+Z
# On your machine:
stty raw -echo; fg
export TERM=xterm
```

---

## :warning: Disclaimer

> This tool is intended for **authorized penetration testing and educational purposes only**. Unauthorized access to computer systems is illegal. Always obtain proper authorization before testing.

---

## :star: Support

If this tool saved you time during a pentest, **give it a star!** It helps others find it.

---

## :page_facing_up: License

MIT License - see [LICENSE](LICENSE) for details.

---

<div align="center">

*Built with :skull: by [Gg](https://github.com/geevarghesekthomas84-sys)*

</div>
