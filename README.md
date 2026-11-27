# 🎧 Universal laut.fm Webplayer V5.2

Ein moderner, responsiver und universeller Webplayer für Radiosender der Plattform **laut.fm**.

Mit diesem Player kann jeder beliebige laut.fm-Sender direkt im Browser abgespielt werden. Einfach den gewünschten Stationsnamen eingeben oder über einen URL-Parameter übergeben – der Player lädt automatisch die passenden Senderinformationen und verbindet sich mit dem zugehörigen Audiostream.

🌐 **Live-Demo:** https://lfm-player.github.io/stream.laut.fm/

**Die Verwendung erfolgt auf eigene Gefahr!**

---

## ✨ Funktionen

### 📻 Universalität und Senderinformationen

- **Universell:** Unterstützt unterschiedliche laut.fm-Sender über ihren Stationsnamen.
- **Automatische Sendererkennung:** Der offizielle Sendername und weitere Stationsinformationen werden über die laut.fm-API geladen.
- **Dynamischer Senderwechsel:** Der gewünschte Sender kann direkt über die Eingabe oder einen URL-Parameter ausgewählt werden.
- **Dynamischer Browser-Titel:** Der offizielle Sendername wird mit „| Webplayer“ kombiniert.
- **Senderlogo als Favicon:** Das Logo des ausgewählten Senders wird dynamisch als Browser-Favicon verwendet.

### 🎵 Musikwiedergabe und Titelinformationen

- **Direkte Stream-Wiedergabe:** Verbindung zum jeweiligen laut.fm-Audiostream.
- **Aktuelle Musikinformationen:** Anzeige von Interpret und Songtitel.
- **Coveranzeige:** Das verfügbare Künstler- beziehungsweise Titelbild wird angezeigt.
- **Senderlogo als Ersatz:** Wenn kein passendes Cover verfügbar ist, wird das Senderlogo verwendet.
- **Play/Pause:** Die Wiedergabe lässt sich bequem steuern.
- **Manuelle Pause:** Eine bewusst ausgelöste Pause verhindert die automatische Wiederaufnahme durch die Wiederverbindungslogik.

### 🔄 Audio-Watchdog und automatische Wiederverbindung

- **Audio-Watchdog:** Überwacht den Fortschritt der Audiowiedergabe.
- **Fehlererkennung:** Erkennt, wenn der Audiostream nicht mehr ordnungsgemäß voranschreitet.
- **Automatischer Reconnect:** Versucht bei Wiedergabeproblemen selbstständig, die Verbindung wiederherzustellen.
- **Gestaffelte Wiederverbindung:** Die erneuten Verbindungsversuche erfolgen nach 2, 4 und 6 Sekunden.
- **Puffer-Reset:** Vor einem erneuten Wiedergabeversuch wird die bisherige Audioquelle entfernt und der Stream neu geladen.
- **Cache-Buster:** Eine neue Stream-URL unterstützt das Anfordern einer frischen Verbindung.

### 🎧 Media Session und Bluetooth

- **Media Session API:** Integration in die Mediensteuerung des Browsers und Betriebssystems.
- **Bluetooth-Steuerung:** Unterstützung der Wiedergabe- und Pausensteuerung über kompatible Bluetooth-Geräte.
- **Titelinformationen:** Übermittlung von Interpret und Songtitel an die Mediensteuerung.
- **Albuminformationen:** Werden nicht separat übertragen. Falls eine Albumangabe benötigt wird, wird stattdessen der Sendername angezeigt.
- **Coveranzeige:** Künstlerbild beziehungsweise Senderlogo als Ersatzbild.
- **Mediensteuerung:** Unterstützung der verfügbaren Play-, Pause- und Stop-Aktionen.

Die tatsächliche Unterstützung einzelner Funktionen hängt vom Browser, Betriebssystem und verwendeten Wiedergabegerät ab.

### 🎨 Design und Anpassungsmöglichkeiten

- **Responsives Design:** Optimiert für Desktop, Tablet und Smartphone.
- **Farbkonfiguration:** Anpassbare Farben für die Gestaltung des Players.
- **URL-basierte Einstellungen:** Individuelle Farbeinstellungen können über die URL weitergegeben und nach einem Neuladen beibehalten werden.
- **Dynamische Gestaltung:** Die Bedienelemente passen sich den gewählten Akzentfarben an.
- **Animationen:** Dezente Hover- und Touch-Effekte.

---

## 🚀 Verwendung

1. Webplayer öffnen.
2. Den gewünschten laut.fm-Stationsnamen eingeben.
3. Auf **Sender öffnen** klicken.
4. Der Player lädt die Senderinformationen und den aktuellen Titel.
5. Die Wiedergabe startet automatisch, sofern der Browser dies erlaubt. Andernfalls kann sie manuell gestartet werden.
6. Die Wiedergabe kann jederzeit pausiert und fortgesetzt werden.

### Direkter Aufruf über die URL

Ein Sender kann auch direkt über den URL-Parameter `station` übergeben werden.

Beispiel:

`https://lfm-player.github.io/stream.laut.fm/?station=eins`

Dabei wird der Sender `eins` automatisch geladen.

---

## 🔧 Verwendete Technologien

- HTML5
- CSS3
- JavaScript
- HTML5 Audio API
- Media Session API
- laut.fm-API
- laut.fm-Audiostreaming
- GitHub Pages

Der Player benötigt keine eigene Datenbank und kein PHP-Backend. Die Anwendung läuft vollständig clientseitig im Browser.

---

## 📡 Datenquellen

Die Senderinformationen und Musiktitel werden über die öffentliche laut.fm-API abgerufen.

API-Endpunkte:

- **Senderinformationen:** `https://api.laut.fm/station/{station}`
- **Aktueller Titel:** `https://api.laut.fm/station/{station}/current_song`
- **Weitere Sender- und Bildinformationen:** `https://api.laut.fm/station/{station}/`

Die Audiowiedergabe erfolgt direkt über den jeweiligen laut.fm-Stream.

Weitere Informationen zur API:

https://docs.api.laut.fm/

---

## 🌍 Hosting

Der Webplayer wird über **GitHub Pages** bereitgestellt.

Das Projekt ist als statische Website umgesetzt und benötigt keinen eigenen Webserver mit serverseitiger Programmlogik.

---

## 🔒 Datenschutzhinweise

Dieses Projekt verwendet die öffentliche laut.fm-API, um Informationen zum ausgewählten Radiosender und zum aktuell gespielten Titel abzurufen.

Bei der Nutzung des Players wird außerdem eine Verbindung zum jeweiligen laut.fm-Audiostream hergestellt.

Im Rahmen dieser Verbindungen können technische Informationen an die jeweiligen Dienste übertragen werden. Dazu gehören insbesondere die IP-Adresse, Informationen zum verwendeten Webbrowser, das Betriebssystem und weitere technisch erforderliche Verbindungsdaten.

Die Datenübertragung erfolgt im Rahmen der technischen Nutzung der laut.fm-Dienste.

Weitere Informationen zur Verarbeitung personenbezogener Daten durch laut.fm findest du unter:

https://laut.fm/pages/privacy

---

## ⚖️ Rechtliche Hinweise

Dieses Projekt ist ein eigenständiges, nicht kommerzielles Hobbyprojekt und wird unabhängig unter dem Namen **lfm-player** entwickelt und bereitgestellt.

Es besteht keine offizielle Verbindung, Partnerschaft oder Zusammenarbeit mit laut.fm, LAUT AG oder GitHub. Das Projekt wird von diesen Unternehmen weder unterstützt noch offiziell empfohlen.

Alle genannten Marken, Produktnamen und Dienstleistungsbezeichnungen sind Eigentum der jeweiligen Rechteinhaber.

**lfm-player – ein unabhängiger Universalplayer für laut.fm.**

**Die Verwendung erfolgt auf eigene Gefahr!**
