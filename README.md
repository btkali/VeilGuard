# 🛡️ VeilGuard
> Visibility that fights back — sicurezza intelligente, spiegabile e sotto controllo.

![VeilGuard Logo](docs/img/logo.png)

## 🧩 Cos’è
VeilGuard è una piattaforma di sicurezza che combina **rilevazione comportamentale** e **machine learning** per individuare, spiegare e contenere minacce in tempo reale.

Pensata per analisti SOC, integra:
- un **agent** leggero per endpoint,
- un **backend** per regole e correlazione,
- un **motore ML** per anomalie e spiegazioni,
- e una **dashboard web** per visibilità totale.

---

## ✨ Funzionalità principali
- 🧠 Rilevazione ibrida (regole + AI)
- 🔍 Spiegabilità delle decisioni
- ⚡ Bassa latenza pipeline
- 🔒 Azioni con approvazione
- 🧩 Integrazione OSQuery / Sigma
- 📈 Dashboard moderna

---

## 🏗️ Architettura
```mermaid
flowchart LR
  A[Agent] --> B(Core)
  B --> C[ClickHouse]
  B --> D[ML Service]
  B --> E[Console]
