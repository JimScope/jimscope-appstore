# Ownfoil

Switch library manager with a self-hosted **Tinfoil / CyberFoil** shop.

It scans your games folder (mounted read-only at `/games`), generates the Tinfoil
index automatically and serves it over HTTP on port **8465**.

## Features
- ✅ Serves **NSP, NSZ, XCI and XCZ** (compressed content supported)
- ✅ Works with **Tinfoil**, **CyberFoil** and **Sphaira**
- ✅ Private shop with multi-user authentication (create an admin on first run)
- ✅ Optional `prod.keys` upload for content identification by decryption
- ✅ Automatic library scan + index generation

## Setup
1. Install and open the app.
2. Create the **admin** user.
3. (Optional) Upload your **console keys** in Settings for accurate title detection.
4. In CyberFoil/Tinfoil add a source: `http://<server-ip>:8465` with your credentials.

Your library is mounted **read-only**, so Ownfoil cannot modify or delete your games.

Source: https://github.com/a1ex4/ownfoil
