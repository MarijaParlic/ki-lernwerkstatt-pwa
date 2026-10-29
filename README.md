# KI-Lernwerkstatt

Eine Progressive Web App zum Lernen an der Schnittstelle von Betriebswirtschaft und künstlicher Intelligenz. Die Anwendung läuft direkt im Browser und kann nach dem ersten Laden auch offline genutzt werden.

**[KI-Lernwerkstatt öffnen](https://marijaparlic.github.io/ki-lernwerkstatt-pwa/)**

## Funktionen

- **Karteikarten:** Zehn vorbefüllte Karten zu KI- und BWL-Begriffen, eigene Karten ergänzen und Lernfortschritt markieren.
- **Kostenvergleich:** Frontier- und Mini-/Lokal-Szenarien mit veränderbaren Tokenpreisen, Nutzungszahlen, Fixkosten und Einführungskosten vergleichen. Die voreingestellten Preise sind Beispiele und keine aktuellen Anbieterpreise. Die Amortisationsdauer wird bei positiver monatlicher Ersparnis berechnet.
- **Notizen und Sicherung:** Lernstand, eigene Karten, Notizen und Rechnerwerte lokal speichern sowie als JSON exportieren und importieren. Ein Import ersetzt die bisherigen lokalen Daten.
- **Offline und installierbar:** Ein Service Worker speichert die App-Dateien nach dem ersten Online-Aufruf. Die App kann auf unterstützten Geräten zum Startbildschirm hinzugefügt werden.

## Installation auf dem Smartphone

1. Den [Live-Link](https://marijaparlic.github.io/ki-lernwerkstatt-pwa/) mit Internetverbindung öffnen und die App einmal vollständig laden.
2. **iPhone/iPad:** In Safari auf **Teilen → Zum Home-Bildschirm** tippen.
3. **Android:** In Chrome das Menü öffnen und **App installieren** oder **Zum Startbildschirm hinzufügen** wählen.

## Lokal ausführen

Einen lokalen HTTP-Server im Projektordner starten, zum Beispiel mit `python3 -m http.server 8000`, und `http://localhost:8000/` öffnen. Service Worker und Installation benötigen HTTPS oder localhost; ein direktes Öffnen per `file://` aktiviert die Offline-Funktion nicht.

## Datenschutz und Hinweise

Die App verwendet keine externen CDNs oder Tracker. Lernstand und Notizen bleiben im lokalen Browserspeicher des jeweiligen Geräts und werden nicht automatisch synchronisiert. Beim Löschen der Browserdaten können sie verloren gehen; sichere sie regelmäßig mit dem JSON-Export. Der Kostenrechner ist eine vereinfachte Planungshilfe: Qualität, Datenschutz, Steuern und weitere Kosten müssen gesondert berücksichtigt werden. Die Karten zum EU AI Act bieten einen Überblick und keine Rechtsberatung.
