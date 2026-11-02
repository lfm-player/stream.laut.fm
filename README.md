# 🎧 Universal laut.fm Webplayer

Ein kleiner, einfacher, moderner, responsiver Webplayer für Radiosender der Plattform **laut.fm**.

Mit diesem Player kann jeder seinen gewünschten laut.fm-Sender direkt im Browser hören. Einfach den Stationsnamen eingeben, Sender öffnen und Musik genießen.

🌐 **Live-Demo:** https://lfm-player.github.io/stream.laut.fm/

---

## ✨ Funktionen

- **Universell:** Unterstützt unterschiedliche laut.fm-Sender über ihren Stationsnamen.
- **Automatische Sendererkennung:** Offizieller Sendername wird über die laut.fm-API geladen.
- **Aktuelle Musikinformationen:** Anzeige von Interpret und Songtitel.
- **Coveranzeige:** Künstlerbild wird angezeigt, sofern verfügbar.
- **Senderlogo als Ersatz:** Wenn kein passendes Songbild vorhanden ist, wird das Logo des ausgewählten Senders verwendet.
- **Direkte Stream-Wiedergabe:** Verbindung zum jeweiligen laut.fm-Audiostream.
- **Automatischer Wiedergabeversuch:** Der Player versucht nach dem Öffnen eines Senders die Wiedergabe zu starten. Die Browser-Autoplay-Regeln können einen manuellen Start erforderlich machen.
- **Play/Pause:** Wiedergabe bequem steuern.
- **Dynamischer Browser-Titel:** Der offizielle Sendername wird mit „| Webplayer“ kombiniert.
- **Responsive Design:** Optimiert für Desktop, Tablet und Smartphone.
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
- laut.fm API
- laut.fm Audio-Streaming
- GitHub Pages

Der Player benötigt keine eigene Datenbank und kein PHP-Backend.

## 📡 Datenquellen

Die Senderinformationen und Musiktitel werden über die offizielle laut.fm-API abgerufen.

API-Endpunkte:

- Stationsinformationen: `https://api.laut.fm/station/{station}`
- Aktueller Titel: `https://api.laut.fm/station/{station}/current_song`

Die Audiowiedergabe erfolgt über den jeweiligen laut.fm-Stream.

## 🌍 Hosting

Der Webplayer wird über **GitHub Pages** bereitgestellt.

Das Projekt ist als statische Website umgesetzt und benötigt keinen eigenen Webserver mit serverseitiger Programmlogik.

## 📄 Lizenz und Hinweise

Dieses Projekt ist ein unabhängiges Webplayer-Projekt zur Wiedergabe von laut.fm-Radiosendern.

laut.fm ist eine eigenständige Plattform. Markenrechte und Rechte an den bereitgestellten Inhalten verbleiben bei den jeweiligen Rechteinhabern.

Die Verfügbarkeit der Senderinformationen, Coverbilder und Audiostreams hängt von laut.fm und den jeweiligen Datenquellen ab.

---

**Universal laut.fm Webplayer**  
*Einfach Sender auswählen. Einschalten. Musik genießen. 🎶*
