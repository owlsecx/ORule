# 🦉 ORule

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OForensics-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-2.0-cyan?style=flat-square"/>
</p>

> **ORule** — Firewall Rule Change Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

ORule is a forensics-grade firewall rule change auditor. It captures a baseline of nftables, iptables, ip6tables or ufw rules and diffs the live configuration against it, scoring changes by risk and recording a JSONL timeline. It supports continuous monitoring, tamper detection and syslog export.

---

## ✨ Features

- Supports nftables, iptables, ip6tables and ufw engines (auto-detected)
- Baseline creation, refresh and diffing against the live ruleset
- Risk scoring with a configurable minimum display level
- Continuous monitoring with a configurable interval and tamper detection
- JSONL timeline, snapshot rotation and snapshot-to-snapshot diffing
- CSV/HTML export, syslog forwarding and a high-risk open-port scan

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./ORule --audit
./ORule --baseline
./ORule --watch 60 --risk HIGH
./ORule --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
