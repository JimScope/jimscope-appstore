Minecraft RAD3 runs the **Roguelike Adventures and Dungeons 3** CurseForge modpack on Minecraft 1.20.1 (Forge), powered by the [itzg/minecraft-server](https://github.com/itzg/docker-minecraft-server) image.

On first boot the container downloads and installs the full modpack automatically, so the initial startup takes several minutes. Watch the logs to follow progress.

## Requirements

- A free **CurseForge API key** (console.curseforge.com → API Keys). It is required to download the modpack.
- At least **6 GB** of RAM allocated (8 GB recommended for a full group). Make sure the host has enough free memory.

## Notes

- The server runs in **offline mode** (`ONLINE_MODE=false`), so no Microsoft/Mojang accounts are needed. Players are identified by username only.
- Because of offline mode, fill the **Whitelist** with your players' exact usernames and enable **Enforce whitelist** to prevent username spoofing of operators.
- Add players live from the console: `rcon-cli whitelist add <name>`.
- This is a TCP game server, not a web app — connect from the Minecraft client using `host:25565`. The Runtipi "open" button does not apply.

Game data is stored under the app data directory in `/data`.
