# A1-Oeffentlich

Öffentliche, statische Seiten der Automation-One GmbH (GitHub Pages).

**Regel:** Nur Inhalte, die jeder sehen darf – keine Zugangsdaten, keine Kundendaten, keine internen Dokumente.

| Adresse | Inhalt | Quelle / Zweck |
|---|---|---|
| https://messkoffer.automation-one.de | Hinweis „Bitte zuerst mit dem Gateway verbinden“ | Erscheint, wenn jemand QR 2 eines A1-Koffer-Gateways scannt, ohne im Gateway-WLAN zu sein. Im Gateway-WLAN beantwortet das Gateway den Namen selbst. Quelle: A1-Customer-Projects/HaustechnikProjekt/Labortests/src/oeffentlich/index.html |

**Aufbau:** GitHub Pages veröffentlicht je Repository eine Website unter einer Adresse (Datei CNAME). Weitere Seiten zu derselben Adresse als Unterordner;
für eine andere Adresse ein weiteres Repository nach demselben Muster (A1-Oeffentlich-<name>).

**Ablauf neue Adresse:** DNS-CNAME <name>.automation-one.de -> a1ki-projects.github.io (IONOS-API, Schlüssel nur auf dem A1-Server),
CNAME-Datei im Repository, Settings › Pages: Branch main / root, Custom domain, Enforce HTTPS.

Schreiben: Deploy-Key des A1-Servers (nur dieses Repository). Stand 20.11.2026.
