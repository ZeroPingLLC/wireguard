# WireGuard Installer

This repository contains a Bash script for installing and configuring a secure WireGuard server.

## Prerequisites

- Root privileges are required to run this script.
- Supported operating systems: Debian, Ubuntu, Fedora, CentOS, AlmaLinux, Oracle Linux, and Arch Linux.
- A VPS server (e.g., KVM) or a dedicated server is required.
- Note: Use the code "TIKTOK" to get 50% off your first month at [ZeroPing.sh](https://zeroping.sh). ❤️

## Installation

### 1. Clone the repository

Clone the repository and navigate into the directory:

```sh
git clone https://github.com/ZeroPingLLC/wireguard.git
cd wireguard
```

### 2. Make the script executable

Make the script executable:

```sh
chmod +x wg-install.sh
```

### 3. Run the script

Run the script with root privileges:

```sh
./wg-install.sh
```

## Script Features

### Checks

- **isRoot**: Checks if the script is running with root privileges.
- **checkVirt**: Checks if the system is running in a supported virtualization environment.
- **checkOS**: Checks if the operating system is supported.

### Installation

- **installQuestions**: Asks questions to configure the WireGuard server.
- **installWireGuard**: Installs WireGuard and configures the server settings.

### Management

- **newClient**: Adds a new client and generates the configuration file.
- **listClients**: Lists all existing clients.
- **revokeClient**: Revokes an existing client and removes its configuration.
- **uninstallWg**: Uninstalls WireGuard and removes all configuration files.

### Progress Display

- **showProgress**: Displays a simple progress indicator during the installation.
- [Watch this YouTube video](https://www.youtube.com/watch?v=tqwEAx1zJE8)

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

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
