# 🦉 OKeycloakX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OKeycloakX** — Offline Keycloak Realm Export & Server Config Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

Offline Keycloak realm export & server configuration auditor

---

## ✨ Features

- Realm settings — sslRequired, brute-force detection, password policy (length / hashIterations / algorithm), registration, verify-email, reset / login-with-email, remember-me, token & session lifespans, offline sessions, refresh-token rotation, OTP policy, required actions, login / admin events, default roles, browser headers
- Clients — public + ROPC, implicit flow, wildcard / http redirect URIs, webOrigins, service accounts holding realm-management roles, full scope, PKCE, inline secrets
- Identity brokering — trustEmail, auto-link first-broker flows, signature validation, inline IdP secrets
- Users & roles — exported credentials, plaintext seeds, realm-admin / impersonation grants, composite escalation
- Server — keycloak.conf / KC_* env / legacy standalone.xml (http-enabled, hostname-strict, proxy headers, db password, metrics / health, /auth relative path, admin hostname, TLS)
- Keycloak version end-of-life detection
- CWE + MITRE ATT&CK + OWASP ASVS mapping, secrets masked
- Client inventory table, score / grade per realm & server
- Export TXT / Markdown / JSON / CSV / SARIF 2.1.0
- Self-test --demo, CI gates --fail-on / --min-severity

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OKeycloakX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
