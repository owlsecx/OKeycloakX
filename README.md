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

OKeycloakX is an offline auditor for Keycloak realm exports and server configuration. It reviews realm-export JSON, `keycloak.conf`, KC_* environment settings, and legacy `standalone.xml` for realm, client, IdP, user/role, and server hardening issues. Findings map to CWE, MITRE ATT&CK, and OWASP ASVS with multi-format export and CI gates.

---

## ✨ Features

- Realm settings: sslRequired, brute-force, password policy, registration, token/session lifespans, OTP, events, headers
- Client checks: public/ROPC, implicit flow, wildcard/http redirect URIs, webOrigins, PKCE, inline secrets, full scope
- Identity brokering: trustEmail, auto-link flows, signature validation, inline IdP secrets
- Users & roles: exported credentials, plaintext seeds, realm-admin/impersonation grants, composite escalation
- Server config via keycloak.conf / KC_* env / standalone.xml (HTTP, hostname-strict, proxy, DB password, metrics/health, TLS)
- Score/grade, client inventory, EOL version hint, TXT/MD/JSON/CSV/SARIF export, `--demo` and fail-on gates

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OKeycloakX --realm realm-export.json --conf keycloak.conf
./OKeycloakX --scan --format sarif -o keycloak.sarif --fail-on high
./OKeycloakX --demo --list-rules
./OKeycloakX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
