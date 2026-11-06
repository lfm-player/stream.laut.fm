# 🎧 Universal laut.fm Webplayer

Ein kleiner, einfacher, moderner und responsiver Webplayer für Radiosender der Plattform **laut.fm**.

Mit diesem Player kann jeder seinen gewünschten laut.fm-Sender direkt im Browser hören. Einfach den Stationsnamen eingeben, Sender öffnen und Musik genießen.

🌐 **Live-Demo:** https://lfm-player.github.io/stream.laut.fm/

Die Verwendung erfolgt auf eigene Gefahr!

---

## ✨ Funktionen

- **Universell:** Unterstützt unterschiedliche laut.fm-Sender über ihren Stationsnamen.
- **Automatische Sendererkennung:** Der offizielle Sendername wird über die laut.fm-API geladen.
- **Aktuelle Musikinformationen:** Anzeige von Interpret und Songtitel.
- **Coveranzeige:** Das Künstlerbild wird angezeigt, sofern verfügbar.
- **Senderlogo als Ersatz:** Wenn kein passendes Songbild vorhanden ist, wird das Logo des ausgewählten Senders verwendet.
- **Direkte Stream-Wiedergabe:** Verbindung zum jeweiligen laut.fm-Audiostream.
- **Automatischer Wiedergabeversuch:** Der Player versucht nach dem Öffnen eines Senders die Wiedergabe zu starten. Die Autoplay-Regeln des Browsers können einen manuellen Start erforderlich machen.
- **Automatischer Reconnect:** Erkennt unerwartete Stream-Unterbrechungen und versucht automatisch, die Verbindung wiederherzustellen. Eine zusätzliche Stream-Überwachung erkennt auch ausbleibenden Audiofortschritt.
- **Play/Pause:** Die Wiedergabe lässt sich bequem steuern. Eine manuelle Pause verhindert die automatische Wiederaufnahme.
- **Dynamischer Browser-Titel:** Der offizielle Sendername wird mit „| Webplayer“ kombiniert.
- **Responsives Design:** Optimiert für Desktop, Tablet und Smartphone.
- **Animationen:** Dezente Hover- und Touch-Effekte.

## 🚀 Verwendung

1. Webplayer öffnen.
2. Den gewünschten laut.fm-Stationsnamen eingeben.
3. Auf **Sender öffnen** klicken.
4. Der Player lädt die Senderinformationen und den aktuellen Titel.
5. Wiedergabe starten oder pausieren.

Beispiel:

`https://lfm-player.github.io/stream.laut.fm/?station=eins`

Der Stationsname kann über den URL-Parameter `station` übergeben werden.

## 🔧 Verwendete Technologien

- HTML5
- CSS3
- JavaScript
- laut.fm-API
- laut.fm-Audiostreaming
- GitHub Pages

Der Player benötigt keine eigene Datenbank und kein PHP-Backend.

## 📡 Datenquellen

Die Senderinformationen und Musiktitel werden über die öffentliche laut.fm-API abgerufen.

API-Endpunkte:

- **Senderinformationen:** `https://api.laut.fm/station/{station}`
- **Aktueller Titel:** `https://api.laut.fm/station/{station}/current_song`
- **Coveranzeige:** `https://api.laut.fm/station/{station}/`

Die Audiowiedergabe erfolgt über den jeweiligen laut.fm-Stream.

## 🌍 Hosting

Der Webplayer wird über **GitHub Pages** bereitgestellt.

Das Projekt ist als statische Website umgesetzt und benötigt keinen eigenen Webserver mit serverseitiger Programmlogik.

## 🔒 Datenschutzhinweise

Dieses Projekt verwendet die öffentliche laut.fm-API, um Informationen zum Sendeplan und zum ausgewählten Radiosender abzurufen.

Beim Zugriff auf die laut.fm-API können technische Informationen an laut.fm übertragen werden. Dazu können insbesondere die IP-Adresse, Informationen zum verwendeten Webbrowser, das Betriebssystem und weitere technische Daten gehören.

Diese Datenübertragung erfolgt im Rahmen der technischen Nutzung der laut.fm-API.

Weitere Informationen zur Verarbeitung personenbezogener Daten findest du in der Datenschutzerklärung und Impressum von laut.fm.

Datenschutzerklärung und Impressum von laut.fm: https://laut.fm/pages/privacy

Weitere Informationen zur laut.fm-API: https://docs.api.laut.fm/

## ⚖️ Rechtliche Hinweise

Dieses Projekt ist ein eigenständiges, nicht kommerzielles Hobbyprojekt und wird unabhängig unter dem Namen **lfm-player** entwickelt und bereitgestellt.

Es besteht keine offizielle Verbindung, Partnerschaft oder Zusammenarbeit mit laut.fm, LAUT AG oder GitHub. Das Projekt wird von diesen Unternehmen weder unterstützt noch offiziell empfohlen.

Alle genannten Marken, Produktnamen und Dienstleistungsbezeichnungen sind Eigentum der jeweiligen Rechteinhaber.

**2026 lfm-player. Die Verwendung erfolgt auf eigene Gefahr!**
