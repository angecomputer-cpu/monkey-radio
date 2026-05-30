# 🐒 Monkey Radio - Video Player Stable (v1.0)

> **Status:** `v1.0 Stable`  
> **Sincronizzazione:** Roma, Italia (Europe/Rome)

Questa è la versione definitiva del video player per il palinsesto dinamico di **Monkey Radio**. Progettata per essere integrata via Iframe, garantisce la sincronizzazione globale dei contenuti.

---

## 🚀 Caratteristiche Principali

* **Palinsesto Dinamico:** Cambio automatico della sorgente video basato sull'orario.
* **Fuso Orario Centralizzato (Roma):** Grazie all'integrazione delle API `Intl`, tutti gli utenti nel mondo vedono lo stesso contenuto sincronizzato sull'ora italiana.
* **Interfaccia Minimalista:** Design "Full Black" ottimizzato per eliminare distrazioni e massimizzare il focus sul video.

---

## 🛠 Migliorie Tecniche

### 📱 Fullscreen & Rotazione
* **Smart Fullscreen:** Tasto dedicato (30x30px) posizionato in basso al centro per una gestione immediata dei permessi browser.
* **Auto-Landscape Force:** All'attivazione dello schermo intero su dispositivi Android, il player forza l'orientamento in **orizzontale**.
* **Anti-Glitch Resize:** Gestione dinamica degli eventi `orientationchange`. Se l'utente ruota fisicamente il telefono, il video si ricalcola istantaneamente per non sparire.

### 🔐 Sicurezza & Iframe
* **Iframe Security Bypass:** Logica ottimizzata per funzionare correttamente all'interno di container (come Nicepage), con gestione degli errori in caso di permessi `allowfullscreen` mancanti.

---

## 📅 Palinsesto Attivo (Orario IT)

| Fascia Oraria | Contenuto Video |
| :--- | :--- |
| **00:00 - 06:00** | Archive Video |
| **06:00 - 09:00** | Certified Video |
| **09:00 - 12:00** | Everyday Video |
| **12:00 - 14:00** | Archive Video |
| **14:00 - 18:00** | Everyday Video |
| **18:00 - 21:00** | Certified Video |
| **21:00 - 00:00** | Everyday Video |

---

### 📥 Integrazione Rapida
Se integri il player in un Iframe, assicurati di includere i permessi necessari:
`allow="fullscreen"` e `allowfullscreen="true"`.

---
*Sviluppato per Monkey Radio. Sorgenti video ospitate su Archive.org.*
