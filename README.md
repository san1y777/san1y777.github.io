SAN1Y OS
### MULTI OS · OPEN SYSTEM · NEXT LEVEL

**Ein unabhängiges Linux-basiertes Betriebssystemprojekt mit einer eigenen High-End-Oberfläche.**

**Entwickler:** Sascha Santori  
**Projektstatus:** Aktive Entwicklung · keine freigegebene stabile Version  
**Projektstand dieser README:** SAN1Y-OS-BACKUP-249-MASTER · 16.11.2026

[🌐 Projektwebseite](https://san1y777.github.io/) · [💻 GitHub-Profil](https://github.com/san1y777) · [✉️ Zusammenarbeit](mailto:san1y777@icloud.com) · [💙 Projekt unterstützen](https://www.paypal.me/sani1y)

</div>

---

## 1. Was ist SAN1Y OS?

**SAN1Y OS** ist ein eigenständiges Betriebssystemprojekt auf Linux-Basis. Das Ziel ist, eine moderne, schnelle und anpassbare Arbeitsumgebung zu schaffen, die hochwertige Gestaltung, Sicherheit, Entwicklerwerkzeuge und – soweit technisch möglich – Anwendungen verschiedener Plattformen zusammenführt.

Im Mittelpunkt stehen **Stabilität, Geschwindigkeit, Sicherheit, Datenschutz und individuelles Design**. Nicht die Anzahl installierter Programme zählt, sondern eine zuverlässig funktionierende, nachvollziehbar getestete Integration.

> **Wichtiger Hinweis:** SAN1Y OS befindet sich in Entwicklung. Die auf der Webseite gezeigten Oberflächen und Bildschirme sind teilweise **Designkonzepte** und kein Beleg für bereits vollständig implementierte Funktionen. Es gibt zum Stand dieses Dokuments **keine als stabil freigegebene öffentliche ISO** und **keinen abschließend getesteten Installationsablauf**.

## 2. Technische Grundlage

| Bereich | Derzeitige Grundlage / Ziel |
|---|---|
| Basis | Ubuntu 24.04 LTS „Noble“ |
| Architektur | x86_64 |
| Desktop | Xfce als bisherige Arbeitsgrundlage |
| Oberfläche | Eigenständiges SAN1Y-Design, in Entwicklung |
| Sprache | Deutsch als geplante Standardsprache; noch nicht überall umgesetzt |
| Terminal | Xfce Terminal im SAN1Y-System |
| Editionen | Standard und Developer Edition vorgesehen |
| Virtualisierung | Schwerpunkt QEMU/KVM |
| Boot | BIOS/UEFI-Bootkonzepte und Tests in früheren Builds |
| Installation | Langfristig sicherer Multiboot neben bestehenden Systemen |

## 3. Gestaltung und Benutzererlebnis

Die Designrichtung heißt **Cyber / Dark Liquid Glass**: dunkle, möglichst transparente Fenster, elektrische blaue Akzente, silberne Menüs, abgerundete Oberflächen und dezente Animationen.

**Vorgesehene Farbpalette:**

| Element | Farbe |
|---|---|
| Hintergrund | `#101114` |
| Fenster | `#1C1D22` |
| Panels | `#25272D` |
| Menüschrift | `#C0C5CE` |
| Terminal | Hintergrund `#080C12`, Schrift `#78FF83` |
| Akzent | Leuchtendes Blau |

**Designziele:**
- Transparente Fenster, Neon-Outlines und ressourcenschonende Effekte
- Modernes Dock **standardmäßig unten**, später verschiebbar
- Anpassbare Icons, Schriftarten, Cursor, Farben und Fenstertransparenz
- Optionaler Hover-Zoom für Desktop-Symbole und Ordner
- Individuelle Desktop-Hintergründe, Login- und Sperrbildschirme
- Eigene Boot- und GRUB-Gestaltung

**Aktueller Stand:** Die visuellen Vorlagen zeigen die beabsichtigte Richtung. Vollständige Umsetzung und Performancetests stehen noch aus.

## 4. Funktionen und Entwicklungsziele

### Personalisierung – SAN1Y Style Studio Pro
Eine grafische Designzentrale mit Farbkreis, HEX-Eingabe, Themes, Import/Export, Transparenz-, Icon-, Cursor-, Schrift- und Dock-Einstellungen, Vorschau und Rückgängig-Funktion.

**Stand:** Ein früher **Style Studio V1**-Starter auf Bash/xmessage-Basis wurde entwickelt und syntaktisch geprüft. Die geplante High-End-GTK-Version ist noch nicht als funktionsfähig bestätigt. Die Akzentfarb-App startet derzeit nicht zuverlässig.

### Developer Hub
Geplant sind Git-Repositories, Klonen, ZIP-Import, Codeeditor, Projektverwaltung, Build-Pipelines, Abhängigkeitsprüfung sowie ein App Maker, Website-zu-App-Konverter und Programmiersprachen-Konverter.

**Stand:** Git, SSH und Mac-Bridge-Funktionen wurden in früheren Live-Systemen getestet; sechs zusätzliche Git-Webstarter sind laut Projektdokumentation eingebunden. Das ist **keine** bestätigte Installation sämtlicher Git-Plattformserver.

### Plattformübergreifende Software
- **Linux:** APT, Flatpak/Flathub, AppImage und geeignete Softwarezentralen
- **Windows:** Prüfung von Wine, Bottles sowie Windows in virtuellen Maschinen
- **Android:** Prüfung von Waydroid beziehungsweise Android-VMs

**Stand:** Breite Windows-/Android-Kompatibilität ist ein Ziel, noch keine zugesicherte Funktion. Windows Store und `winget` wären nur in einer passenden Windows-Umgebung nutzbar.

### Virtuelle Maschinen und Security Lab
QEMU/KVM steht im Zentrum. Geplant sind Windows- und Android-VMs sowie ein **isoliertes Kali Security Lab** für autorisierte Sicherheitsprüfungen und Lernen. Historische BackTrack-Software wird nicht als ungeschützte Produktivumgebung eingesetzt.

**Stand:** Virtualisierungs- und Boot-Tests wurden durchgeführt; neuere grafische Tests und Performanceoptimierungen sind offen.

### Lokale KI und kreative Werkzeuge
Geplant sind lokale KI-Modelle mit geeigneten Laufzeiten wie Ollama/llama.cpp, KI-Chat, Codeassistenz, Bild-/Videowerkzeuge, Prompt-zu-Skript, Video-zu-PDF und Modellverwaltung.

**Stand:** Forschungs- und Integrationsziele; die genannten externen Projekte sind nicht automatisch installiert oder getestet.

### Cloud, Backups und Wiederherstellung
Vorgesehen sind Backups auf interne/externe Datenträger, USB, NAS, private Server und geeignete Cloud-Dienste. Geplant sind inkrementelle und verschlüsselte Backups, Snapshots, Systemabbilder, Restore-Assistenten und echte Wiederherstellungstests.

### Systemgesundheit, Sicherheit und Auto-Fix
Geplant sind Hardwareüberwachung, Paket-/Konfigurationsdiagnose, Integritätsprüfungen, Firewall, Verschlüsselung, Sicherheitswarnungen und **reversible** Reparaturvorschläge. Persönliche Dateien sollen **niemals ungefragt gelöscht** werden.

### Anmeldung und iPhone-Integration
Geplant sind Benutzerkonten, Passwort/PIN-Optionen, ein gestalteter Sperrbildschirm und die Erforschung einer iPhone-gestützten Freigabe. **Face ID über iPhone ist bislang ein Entwicklungsziel, keine funktionierende Linux-Anmeldemethode in SAN1Y OS.**

### Installation, Updates und Multiboot
Langfristiges Ziel ist eine geprüfte Installation neben Windows oder Linux, mit Backup, Prüfung der Partitionstabelle, Schutz bestehender Bootloader und ausdrücklicher Zustimmung für riskante Änderungen. Eine eigene signierte Update-Infrastruktur ist vorgesehen.

**Stand:** Ein realer, vollständig getesteter Multiboot-Installer und ein fertiger eigener Updatekanal sind nicht bestätigt.

## 5. Bisherige Entwicklung und Builds

Die Projektsicherung dokumentiert unter anderem diese Entwicklungsstufen:

| Build / Meilenstein | Dokumentierter Stand |
|---|---|
| Prototyp 135 | Frühe ISO |
| GUI-Test 152 | Grafischer ISO-Test |
| Dark 174 / 179 | Desktop- und Design-Tests |
| Developer 208 | Früher UEFI-QEMU-Test nachgewiesen |
| Developer 221 | BIOS-/UEFI-Tests laut Nutzer erfolgreich |
| Developer 230 | ISO erstellt, BIOS-/UEFI-Booteinträge vorhanden; vollständige Grafik-/UEFI-Gasttests nicht abschließend dokumentiert |
| Rootfs 234 | Auf dem Entwicklungsrechner als vorhanden bestätigt |
| Developer 247 | Build vorbereitet; tatsächlicher Dateibestand, SHA256 und Bootfähigkeit noch nicht verifiziert |

**Technische Referenz für Build 230:** Kernel `6.8.0-149-generic`, SquashFS 4.0 mit XZ-Komprimierung, BIOS-/UEFI-El-Torito-Einträge; Live- und Diagnose-Menü vorhanden. Der dokumentierte SHA256-Wert der ISO lautet:

```text
SAN1Y-OS-DEV-230.iso
1bdcd828788241d1b34edf3e87bfe28be6fb70b4b2fe12cd7ce109a9d5d1668b
```

Der Hash stammt aus der Projektsicherung. Er wurde **nicht im Zuge dieser README unabhängig gegen eine lokale ISO geprüft**.

### Was als bestätigt gilt
- Mehrere frühe ISO- und Rootfs-Entwicklungsstufen
- Vorhandensein von Rootfs 234 und ISO 230 laut bisheriger Projektdokumentation
- BIOS-/UEFI-Booteinträge in ISO 230
- Frühe Tests mit QEMU/UEFI und anderen Bootvarianten
- Style Studio V1 syntaktisch geprüft
- Terminal-Farbprofil in Rootfs 234 erstellt
- Git-/SSH-/Mac-Bridge-Tests aus früheren Entwicklungsphasen

### Was noch nicht als fertig gilt
- Vollständig funktionierende und verifizierte ISO 247
- Komplett deutsche Oberfläche
- Flüssige, reale Bootanimation und endgültiges Login-Design
- Zuverlässiges grafisches Style Studio mit Farbrad
- Windows-/Android-Kompatibilität in der gewünschten Breite
- Vollständiges Kali-Labor, Auto-Fix und iPhone-Entsperrung
- Sicher getesteter Multiboot-Installer und allgemeine Hardwarefreigabe

## 6. Aktuelle Probleme und Prioritäten

| Priorität | Offener Punkt |
|---|---|
| P0 | QEMU-/Simulationsleistung verbessern |
| P0 | Deutsche Sprache konsistent umsetzen |
| P0 | Nicht startende Akzentfarb-App reparieren |
| P0 | Fehlendes SAN1Y-Systemsymbol beheben |
| P0 | Bootgrafik, Animation, Login und Sperrbildschirm implementieren und testen |
| P0 | Terminal-Gast-Zwischenablage und GUI-Tests verbessern |
| P0 | ISO 247 auf Existenz, SHA256 und Bootverhalten prüfen |
| P1 | Farbkreis, Icons, Neonordner, Dock, Widgets und Softwaremanager weiterentwickeln |
| P1 | Sichere Systemdiagnose und Auto-Fix vorbereiten |

## 7. Roadmap

Die Reihenfolge ist **geplant, keine Zusage für Veröffentlichungstermine**.

1. **Stabilität:** Build-Dateien, KVM, ISO-Hashes, Geschwindigkeit, Sprache, GUI und Zwischenablage prüfen.
2. **High-End-Design:** Branding, Bootanimation, Dock, Fenster, Icons und Anmeldung verbessern.
3. **Style Studio Pro:** Grafik-App mit Farbrad, Profilen, Themes und Vorschau.
4. **Softwarezentrale:** Browser, Office/PDF, Multimedia, Kommunikation, Developer Hub und KI-Werkzeuge.
5. **Multiplattform:** Wine/Bottles, Windows-/Android-VMs und isoliertes Security Lab.
6. **Cloud & Sicherheit:** Backups, Verschlüsselung, Updates, Auto-Fix und Wiederherstellung.
7. **Installer:** Überprüfte Dual-/Multiboot-Installation und Hardwaretests.

## 8. Sicherheit und verantwortliche Entwicklung

Bei SAN1Y OS gelten folgende Projektprinzipien:

- Keine Löschung oder Überschreibung alter ISO-/Rootfs-Bestände ohne Zustimmung.
- Keine Veränderung vorhandener Windows-/Linux-Partitionen oder Host-Bootloader ohne ausdrückliche Freigabe.
- Keine automatische Partitionierung und kein ungeprüftes Ausführen fremder Skripte als Root.
- Keine automatische Löschung vermeintlicher Duplikate oder persönlicher Daten.
- Backups, Wiederherstellbarkeit und Rollback vor kritischen Änderungen prüfen.
- Fremdsoftware zunächst hinsichtlich Lizenz, Abhängigkeiten, Berechtigungen und Risiken bewerten.
- Sicherheitswerkzeuge nur für eigene oder ausdrücklich autorisierte Systeme verwenden.
- Den Entwicklungsstatus transparent ausweisen: **geplant ≠ implementiert ≠ getestet ≠ freigegeben**.

## 9. Screenshots und Designvorschauen

Screenshots, Bootgrafiken, das Schloss-Logo und die Desktopkonzepte sind auf der [Projektwebseite](https://san1y777.github.io/) zu sehen. Sie zeigen die **Designvision**. Der technische Implementierungsgrad einzelner dargestellter Funktionen kann davon abweichen.

## 10. Download und Installation

**Aktuell kein allgemein freigegebener stabiler Download.** Bitte verwende Entwicklungs-ISOs nicht ungeprüft auf produktiven Systemen und führe keine Partitionierungs- oder Bootloader-Änderungen ohne Sicherung durch.

Sobald eine Version hinsichtlich Bootverhalten, Prüfsumme, Sicherheit, Installation und Wiederherstellung ausreichend geprüft ist, können offizielle Downloadinformationen und Prüfsummen hier ergänzt werden.

## 11. Zusammenarbeit und Unterstützung

SAN1Y OS wird von **Sascha Santori** entwickelt. Für konstruktive technische Zusammenarbeit, Tests, Designideen und Projektanfragen:

- **E-Mail:** [san1y777@icloud.com](mailto:san1y777@icloud.com)
- **Webseite:** [san1y777.github.io](https://san1y777.github.io/)
- **GitHub:** [san1y777](https://github.com/san1y777)
- **Freiwillig unterstützen:** [PayPal.me/sani1y](https://www.paypal.me/sani1y)

Spenden sind freiwillig und begründen weder einen Anspruch auf Funktionen noch auf einen Veröffentlichungstermin.

## 12. Lizenz und Hinweise

Für dieses Projekt wurde im dokumentierten Stand **keine allgemeine Open-Source-Lizenz festgelegt**. „Open System“ ist der Projektname beziehungsweise die Ausrichtung und stellt **keine automatische Freigabe sämtlicher Dateien zur Nachnutzung** dar. Vor Beiträgen, Forks oder Weiterverteilung sind die tatsächlich im Repository ausgewiesenen Lizenzbedingungen zu prüfen. Rechte an verwendeten Fremdprogrammen, Marken und Logos verbleiben bei den jeweiligen Rechteinhabern.
