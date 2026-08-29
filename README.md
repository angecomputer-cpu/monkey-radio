# 🐒 Monkey Radio - Screensaver Player Stable (v1.1)

**Status:** v1.1 Stable  
**Sincronizzazione:** Roma, Italia (`Europe/Rome`)

Versione aggiornata del player/screensaver per il palinsesto dinamico di **Monkey Radio**. Progettata per l'integrazione via iframe o visualizzazione standalone fullscreen, garantisce la sincronizzazione globale dei contenuti e delle grafiche di scena.

---

## 🚀 Caratteristiche Principali

* **Palinsesto & Grafiche Dinamiche:** Cambio automatico di loghi, sfondi e titoli dello show in base all'orario italiano.
* **Scena Doppia Interattiva (Show / Track):**
  * **Scena 1 (Show):** Animazione typewriter per il nome della radio (*MONKEY RADIO*) e per il titolo dello show attivo.
  * **Scena 2 (Track Metadata):** Transizione fluida alla traccia in onda con recupero dinamico di artista, titolo e cover art ad alta risoluzione (via iTunes API).
* **Marquee Automatico Sincronizzato:** Lo scorrimento del testo (*marquee*) per artista e titolo si attiva **esclusivamente** se la lunghezza della stringa supera la larghezza del contenitore visibile.
* **Fuso Orario Centralizzato (Roma):** Gestione precisa del tempo tramite API `Intl` per sincronizzare tutti gli utenti globalmente.

---

## 🛠 Migliorie Tecniche & Interfaccia

### 📺 Visual & Layout
* **Background Scaling & Clean View:** Iframe YouTube in background con over-scale per eliminare watermark e titoli nativi.
* **Typing Animation:** Effetto comparsa carattere per carattere su stazione e titolo dello show.

### 📱 Fullscreen & UI Control
* **Smart Fullscreen Button:** Tasto dedicato (posizionato in basso al centro) con icone dinamiche di stato (Enter/Exit Fullscreen) e supporto ai permessi dei browser moderni.
* **Responsive Layout:** Adattamento automatico della griglia e delle dimensioni dei font per dispositivi mobile e tablet.

### 🔐 Sicurezza & Iframe
* **Iframe Security Bypass:** Logica ottimizzata per il funzionamento in container terzi (es. Nicepage) con fallback in caso di restrizioni sui permessi fullscreen.

---

## 📅 Palinsesto & Show Attivi (Orario IT)

| Fascia Oraria | Format / Titolo Show | Logo & Asset |
| :--- | :--- | :--- |
| **00:00 - 06:00** | *Monkey Archive* | Logo Archive |
| **06:00 - 09:00** | *Monkey House Certified* | Logo Certified |
| **09:00 - 12:00** | *Monkey House Everyday* | Logo Everyday |
| **12:00 - 14:00** | *Monkey Archive* | Logo Archive |
| **14:00 - 18:00** | *Monkey House Everyday* | Logo Everyday |
| **18:00 - 21:00** | *Monkey House Certified* | Logo Certified |
| **21:00 - 00:00** | *Monkey House Everyday* | Logo Everyday |

---

## 📥 Integrazione Rapida

Se integri il player all'interno di un `<iframe>`, assicurati di includere i permessi corretti per il supporto fullscreen:

```html
<iframe src="PATH_DEL_TUO_PLAYER.html" 
        width="100%" 
        height="100%" 
        style="border:none;" 
        allow="autoplay; fullscreen" 
        allowfullscreen="true">
</iframe>
