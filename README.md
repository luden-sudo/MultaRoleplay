# MultaRoleplay

![Java](https://img.shields.io/badge/Java-8-ED8B00?logo=openjdk&logoColor=white)
![Spigot](https://img.shields.io/badge/Spigot-1.12%2B-orange)
![Version](https://img.shields.io/badge/version-1.5-blue)
[![SpigotMC](https://img.shields.io/badge/download-SpigotMC-ED8106)](https://www.spigotmc.org/resources/multa-roleplay.108668/)

A **Minecraft roleplay plugin** that lets police/staff issue **fines (multas)** to players and keeps a full history of every fine.

## Features

- 🚓 Fine online players with an amount and a reason
- 📜 Per-player fine history: date, amount, reason and issuing officer
- ⌨️ Tab-completion for every command
- 🔐 Permission-based access
- 🌍 Fully configurable messages with `&` color codes
- 🔄 In-game config reload

## Commands

| Command | Description | Permission |
| --- | --- | --- |
| `/multa <player> <amount> <reason>` | Fine a player | `luden-multa.multa` |
| `/multa reload` | Reload the configuration | `luden-multa.multa` |
| `/multahistory <player>` | Show a player's fine history | `luden-multa.history` |

## Installation

1. Download the latest release from [SpigotMC](https://www.spigotmc.org/resources/multa-roleplay.108668/).
2. Drop the `.jar` into your server's `plugins/` folder.
3. Restart the server and edit `plugins/MultaRoleplay/config.yml` to your liking.

## Configuration

```yaml
Formato: "&cUso: /multa &a<Jugador> <Cantidad> <Razon>"
Cantidad-Invalida: "&c¡Cantidad Invalida!"
Sin-Permisos: "&cNo tienes permiso"
```

## Build from source

```bash
mvn clean package
```

The plugin jar is generated in `target/`.

## Tech stack

Java · Spigot API · Maven

---

Made by [Luden](https://github.com/ludenelenterrador)
