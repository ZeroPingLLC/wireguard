# WireGuard Installer

Dieses Repository enthält ein Bash-Skript zur Installation und Konfiguration eines sicheren WireGuard-Servers.

## Voraussetzungen

- Root-Rechte werden benötigt, um dieses Skript auszuführen.
- Unterstützte Betriebssysteme: Debian, Ubuntu, Fedora, CentOS, AlmaLinux, Oracle Linux und Arch Linux.
- Erforderlich ist ein VPS-Server, z.B. KVM, oder ein dedizierter Server.
- Hinweis: Mit dem Code "TIKTOK" erhältst du bei [ZeroPing.sh](https://zeroping.sh) im ersten Monat 50% Rabatt ❤️

## Installation

### 1. Repository klonen

Klonen Sie das Repository und navigieren Sie in das Verzeichnis:

```sh
git clone https://github.com/ZeroPingLLC/wireguard.git
cd wireguard
```

### 2. Skript ausführbar machen

Machen Sie das Skript ausführbar:

```sh
chmod +x wg-install.sh
```

### 3. Skript ausführen

Führen Sie das Skript mit root-Rechten aus:

```sh
./wg-install.sh
```

## Funktionen des Skripts

### Überprüfungen

- **isRoot**: Überprüft, ob das Skript mit Root-Rechten ausgeführt wird.
- **checkVirt**: Überprüft, ob das System in einer unterstützten Virtualisierungsumgebung läuft.
- **checkOS**: Überprüft, ob das Betriebssystem unterstützt wird.

### Installation

- **installQuestions**: Stellt Fragen zur Konfiguration des WireGuard-Servers.
- **installWireGuard**: Installiert WireGuard und konfiguriert die Servereinstellungen.

### Verwaltung

- **newClient**: Fügt einen neuen Client hinzu und generiert die Konfigurationsdatei.
- **listClients**: Listet alle existierenden Clients auf.
- **revokeClient**: Widerruft einen bestehenden Client und entfernt dessen Konfiguration.
- **uninstallWg**: Deinstalliert WireGuard und entfernt alle Konfigurationsdateien.

### Fortschrittsanzeige

- **showProgress**: Zeigt eine einfache Fortschrittsanzeige während der Installation.

```
printf "${GREEN}
   .--.
  |o_o |
  |:_/ |
 //   \\ \\
(|     | )
/'\\_   _/`\\
\\___)=(___/
${NC}\n"
```

## Lizenz

Dieses Projekt ist lizenziert unter der MIT-Lizenz - siehe die [LICENSE](LICENSE) Datei für Details.
