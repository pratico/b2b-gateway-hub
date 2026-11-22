# b2b-gateway-hub — Fault-Tolerant B2B API Gateway & Asynchronous ETL Middleware

🇬🇧 / 🇺🇸 **ENGLISH** | [🇮🇹 Vai alla versione in Italiano](#-italiano)

[![Portfolio](https://img.shields.io/badge/Portfolio-antoniangeloflore.com-0d6efd?style=flat-square)](https://antoniangeloflore.com)
[![Environment](https://img.shields.io/badge/Production-Live%20on%20Linux%20VPS-198754?style=flat-square)](https://antoniangeloflore.com)
[![Stack](https://img.shields.io/badge/Stack-Node.js%20%7C%20Express%20%7C%20MySQL%20%7C%20Linux-212529?style=flat-square)](https://github.com/pratico)
[![Privacy](https://img.shields.io/badge/Compliance-GDPR%20Safe%20%2F%20Zero--PII-dc3545?style=flat-square)](https://antoniangeloflore.com)

## 📌 Product Overview

**b2b-gateway-hub** is a production-grade **B2B API Gateway, ETL middleware, and asynchronous connector hub** engineered for **SMEs, web agencies, and e-commerce operations** that need to synchronize data flows across ERPs, storefronts, and external webhooks without losing orders or exposing sensitive data.

Deployed and running live on a **dedicated Linux VPS**, it acts as a fault-tolerant traffic controller: incoming payloads are validated, normalized, deduplicated, and routed asynchronously to downstream systems—eliminating manual data entry and silent webhook failures.

## 🎥 Live VPS Production & `b2b-dlq-hub` Integration Demo

* **Live Architecture Benchmark:** **b2b-gateway-hub** is actively deployed on a Linux VPS and showcased in live technical video pitches working in tandem with [**b2b-dlq-hub**](https://github.com/pratico/b2b-dlq-hub) to ingest, route, and stress-test real payload streams under simulated endpoint failures.
* **Watch the Video Pitch & Live Demos:** [https://antoniangeloflore.com](https://antoniangeloflore.com) *(Note: The portfolio portal and the two embedded technical video pitches are currently in Italian, while B2B engineering delivery, documentation, and asynchronous support are fully available in English).*

## 🎯 The Problem Solved

In real-world B2B and e-commerce operations, fragile integrations and manual data transfers create costly bottlenecks:

* **Silent Webhook & Order Losses:** When an external ERP or store API slows down or returns a `502/504` timeout, standard integrations drop payloads permanently.
* **Race Conditions & Duplicate Processing:** Concurrent webhook retries often create duplicate orders or corrupted inventory counts.
* **Manual Data Transcoding:** Teams waste hours every week manually moving and reformatting CSV/XML/JSON records between spreadsheets, ERPs, and online platforms.
* **Single-Operator Bottlenecks:** Mission-critical synchronization depends on fragile scripts or manual intervention.

**b2b-gateway-hub** removes these points of failure: data enters once through a protected gateway, is processed asynchronously with built-in fault tolerance, and reaches every target system reliably.

## ⚙️ Operator & System Workflow

The workflow is designed for zero manual friction once configured:

1. **Controlled Ingestion** — External systems, webhooks, or operators submit payloads to the gateway via hardened REST endpoints or guided web interfaces.
2. **Validation, Deduplication & ETL Normalization** — The engine sanitizes, maps, and validates incoming records according to deterministic business rules before any downstream write occurs.
3. **Asynchronous Routing & Single-Flight Protection** — Requests are queued and dispatched asynchronously, preventing race conditions and traffic spikes from overwhelming target ERPs or databases.
4. **Full Traceability & Replay** — Every transaction is logged in MySQL with real-time status visibility, enabling instant inspection and safe idempotent replay in case of downstream downtime.

## 🚀 Key Capabilities & Operational ROI

* **End-to-End Asynchronous Automation:** Eliminates repetitive manual data transfers across disconnected business platforms.
* **Fault Tolerance & Zero Lost Payloads:** Built-in retry mechanisms and integration with **b2b-dlq-hub** ensure operational continuity even when third-party APIs go offline.
* **High-Concurrency Stability:** Engineered to absorb traffic bursts without blocking the main event loop or corrupting state.
* **Responsive Control Interface:** Clean Bootstrap 5 dashboard accessible from desktop and mobile for real-time queue monitoring.
* **Immediate ROI & Single-Operator Leverage:** A single technical operator can govern high-volume data pipelines that would otherwise require dedicated administrative staff, paying back deployment costs within the first weeks.

## 🛠️ High-Level Technology Stack

* **Node.js & Express** — Non-blocking, event-driven runtime engineered for high-concurrency webhook ingestion and asynchronous queue workers.
* **MySQL** — Battle-tested relational persistence for transactional logs, payload state tracking, and idempotency keys.
* **Bootstrap 5** — Lightweight, responsive operational dashboard with zero frontend bloat.
* **Linux VPS (PM2 / Nginx)** — Hardened production deployment for continuous 24/7 unattended execution.

## 🔒 Confidentiality Notice & B2B Collaboration

🔒 **Proprietary Software Asset (All Rights Reserved)**: This repository serves as a functional and architectural showcase within the Professional Portfolio (https://antoniangeloflore.com — **note:** *video pitches are currently in Italian; both the portfolio portal and B2B technical delivery are available in English*). For operational security and NDA compliance, the source code and internal packaging are not publicly exposed.
* 
* **Custom B2B Integrations & Free 50-Row / Payload Evaluation:** Available for custom API/Webhook stabilization, high-volume ETL pipelines, and white-label licensing via an **asynchronous, zero-call workflow**. Connect on [LinkedIn](https://www.linkedin.com/in/antoniangelo-f-30003622/) or reach out through [antoniangeloflore.com](https://antoniangeloflore.com).

---

<a name="-italiano"></a>
## 🇮🇹 ITALIANO

# b2b-gateway-hub — Gateway API B2B Tollerante ai Guasti & Middleware ETL Asincrono

## 📌 Panoramica del Prodotto

**b2b-gateway-hub** è un **API Gateway B2B, middleware ETL e hub di connettori asincroni** progettato per **PMI, web agency e team e-commerce** che necessitano di sincronizzare flussi di dati tra gestionali (ERP), store online e webhook esterni senza perdere ordini né esporre dati sensibili.

Attivo e funzionante in produzione su **VPS Linux dedicato**, opera come centrale di smistamento resiliente: i payload in ingresso vengono validati, normalizzati, deduplicati e instradati in modalità asincrona verso i sistemi di destinazione, azzerando il data-entry manuale e i guasti silenziosi delle API.

## 🎥 Ambiente Live su VPS & Demo di Integrazione con `b2b-dlq-hub`

* **Architettura Verificata in Produzione:** **b2b-gateway-hub** è installato e operativo su VPS Linux e viene mostrato nei Video Pitch tecnici in sinergia con [**b2b-dlq-hub**](https://github.com/pratico/b2b-dlq-hub) per ricevere, instradare e testare flussi di dati reali simulando guasti e picchi di carico.
* **Guarda i Video Pitch e le Demo Tecniche:** [https://antoniangeloflore.com](https://antoniangeloflore.com)

## 🎯 Il Problema Risolto

Nella gestione operativa quotidiana di PMI e progetti e-commerce, integrazioni fragili e passaggi manuali generano costi nascosti e blocchi operativi:

* **Perdita Silenziosa di Ordini e Webhook:** Quando un gestionale o un'API esterna rallenta o va in timeout (`502/504`), le integrazioni standard perdono i dati trasmessi.
* **Race Condition e Duplicazioni:** I tentativi simultanei di reinvio dei webhook generano ordini duplicati o disallineamenti di magazzino.
* **Trascodifica Manuale dei Dati:** Ore perse ogni settimana a spostare e formattare tracciati CSV/XML/JSON tra fogli di calcolo, ERP e piattaforme web.
* **Colli di Bottiglia Operativi:** Flussi critici bloccati da script fragili o dalla necessità di intervento manuale.

**b2b-gateway-hub** elimina questi attriti: i dati entrano una sola volta attraverso un gateway protetto, vengono elaborati in modo asincrono con tolleranza ai guasti integrata e raggiungono ogni destinazione in sicurezza.

## ⚙️ Come Funziona (Flusso Operativo)

1. **Acquisizione Controllata** — Sistemi esterni, webhook o operatori inviano i dati al gateway tramite endpoint REST protetti o interfacce guidate.
2. **Validazione, Deduplicazione e Normalizzazione ETL** — Il motore sanitizza, mappa e valida i record secondo regole deterministiche prima di qualsiasi scrittura a valle.
3. **Instradamento Asincrono & Protezione Single-Flight** — Le richieste vengono accodate e smistate in modo asincrono, evitando che picchi di traffico o richieste concorrenti mandino in blocco i sistemi destinatari.
4. **Tracciabilità Completa e Replay Idempotente** — Ogni transazione è registrata su MySQL con stato consultabile in tempo reale, permettendo verifiche immediate e il replay sicuro in caso di indisponibilità temporanea degli endpoint esterni.

## 🚀 Funzionalità Principali & Vantaggi Operativi (ROI)

* **Automazione End-to-End:** Riduzione drastica dei tempi di gestione e sincronizzazione manuale dei dati.
* **Tolleranza ai Guasti & Zero Dati Persi:** Meccanismi di retry integrati e interoperabilità nativa con **b2b-dlq-hub** per garantire continuità operativa anche in caso di anomalie esterne.
* **Stabilità ad Alta Concorrenza:** Progettato per assorbire picchi di richieste senza bloccare i processi né corrompere i dati.
* **Interfaccia Responsive:** Pannello di controllo Bootstrap 5 consultabile da desktop e mobile senza curva di apprendimento.
* **ROI Immediato & Leva Singolo Operatore:** Un solo operatore tecnico può governare volumi di flussi che richiederebbero personale dedicato, ripagando l'investimento nelle prime settimane.

## 🛠️ Tecnologie Utilizzate (Ad Alto Livello)

* **Node.js & Express** — Runtime asincrono ad alte prestazioni per la gestione di webhook concorrenti e worker in coda.
* **MySQL** — Database relazionale consolidato per log transazionali, tracciamento stati e chiavi di idempotenza.
* **Bootstrap 5** — Interfaccia operativa leggera, responsive e immediata.
* **VPS Linux (PM2 / Nginx)** — Infrastruttura di produzione per esecuzione continua 24/7.

## 🔒 Nota di Riservatezza & Collaborazioni B2B

* **Asset Software Proprietario (Tutti i diritti riservati):** Questo repository ha finalità di presentazione funzionale e architetturale per il Portfolio Professionale ([https://antoniangeloflore.com](https://antoniangeloflore.com)). Per ragioni di sicurezza operativa e accordi di riservatezza (NDA), il codice sorgente di produzione e le specifiche infrastrutturali non sono esposti pubblicamente.
* **Integrazioni B2B Custom & Test Gratuito:** Disponibile per messa in sicurezza di flussi API/Webhook, pipeline ETL ad alto volume e licenze White-Label con **operatività 100% asincrona (zero call)**. Contattami su [LinkedIn](https://www.linkedin.com/in/antoniangelo-f-30003622/) o tramite [antoniangeloflore.com](https://antoniangeloflore.com).
