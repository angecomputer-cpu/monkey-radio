<!DOCTYPE html>
<html lang="it">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>README - Monkey Radio Player v1 Stable</title>
    <style>
        :root {
            --monkey-yellow: #ffcc00;
            --bg-dark: #121212;
            --card-bg: #1e1e1e;
            --text-main: #e0e0e0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--text-main);
            background-color: var(--bg-dark);
            margin: 0;
            padding: 20px;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            background: var(--card-bg);
            padding: 40px;
            border-radius: 12px;
            border-left: 5px solid var(--monkey-yellow);
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
        }

        h1 {
            color: var(--monkey-yellow);
            border-bottom: 2px solid #333;
            padding-bottom: 10px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        h2 {
            color: var(--monkey-yellow);
            margin-top: 30px;
            display: flex;
            align-items: center;
        }

        h2::before {
            content: '🐒';
            margin-right: 10px;
        }

        ul {
            list-style: none;
            padding-left: 0;
        }

        li {
            margin-bottom: 12px;
            padding-left: 25px;
            position: relative;
        }

        li::before {
            content: '✔';
            position: absolute;
            left: 0;
            color: var(--monkey-yellow);
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
            background: #252525;
            border-radius: 8px;
            overflow: hidden;
        }

        th, td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid #333;
        }

        th {
            background-color: var(--monkey-yellow);
            color: #000;
            text-transform: uppercase;
            font-size: 0.9em;
        }

        tr:hover {
            background-color: #2a2a2a;
        }

        .badge {
            display: inline-block;
            background: var(--monkey-yellow);
            color: #000;
            padding: 2px 10px;
            border-radius: 4px;
            font-weight: bold;
            font-size: 0.8em;
            margin-bottom: 20px;
        }

        footer {
            margin-top: 40px;
            font-size: 0.8em;
            text-align: center;
            color: #666;
        }
    </style>
</head>
<body>

    <div class="container">
        <span class="badge">v1.0 Stable</span>
        <h1>Monkey Radio Player</h1>
        <p>Documentazione tecnica del player video dinamico per il palinsesto di Monkey Radio.</p>

        <h2>Caratteristiche Principali</h2>
        <ul>
            <li><strong>Palinsesto Dinamico:</strong> Cambio automatico della sorgente video basato sull'orario.</li>
            <li><strong>Fuso Orario Centralizzato:</strong> Sincronizzazione globale sull'ora di <strong>Roma (Europe/Rome)</strong> tramite API Intl.</li>
            <li><strong>Esperienza Seamless:</strong> Design Black Screen ottimizzato per autoplay e loop infinito.</li>
        </ul>

        <h2>Migliorie Tecniche (v1 Stable)</h2>
        <ul>
            <li><strong>Smart Fullscreen:</strong> Tasto dedicato 30x30px con gestione attiva dei permessi browser.</li>
            <li><strong>Auto-Landscape:</strong> Forzatura dell'orientamento orizzontale su dispositivi Android all'avvio del fullscreen.</li>
            <li><strong>Iframe Ready:</strong> Logica di bypass per le restrizioni di sicurezza degli iframe (allowfullscreen).</li>
            <li><strong>Anti-Glitch Resize:</strong> Gestione degli eventi <em>orientationchange</em> per evitare la sparizione del video durante la rotazione fisica del dispositivo.</li>
        </ul>

        <h2>Palinsesto Attivo</h2>
        <table>
            <thead>
                <tr>
                    <th>Orario (IT)</th>
                    <th>Contenuto Video</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>00:00 - 06:00</td>
                    <td>Archive Video</td>
                </tr>
                <tr>
                    <td>06:00 - 09:00</td>
                    <td>Certified Video</td>
                </tr>
                <tr>
                    <td>09:00 - 12:00</td>
                    <td>Everyday Video</td>
                </tr>
                <tr>
                    <td>12:00 - 14:00</td>
                    <td>Archive Video</td>
                </tr>
                <tr>
                    <td>14:00 - 18:00</td>
                    <td>Everyday Video</td>
                </tr>
                <tr>
                    <td>18:00 - 21:00</td>
                    <td>Certified Video</td>
                </tr>
                <tr>
                    <td>21:00 - 00:00</td>
                    <td>Everyday Video</td>
                </tr>
            </tbody>
        </table>

        <footer>
            Sviluppato per Monkey Radio. Tutti i diritti sui contenuti video appartengono ai rispettivi proprietari su Archive.org.
        </footer>
    </div>

</body>
</html>
