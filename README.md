# La Fabrik — Releases

Binaires + manifest d'auto-update pour **La Fabrik**.

➡️ **Code source** : <https://github.com/HydrowZer/Hydrowapp>
➡️ **Dernière version** : <https://github.com/HydrowZer/lafabrik-releases/releases/latest>

## Téléchargements

À chaque release, ce repo contient :

- `*.dmg` — installateur macOS (universel x86_64 + aarch64)
- `*.app.tar.gz` + `*.sig` — bundle consommé par l'updater Tauri (macOS)
- `*.msi` — installateur Windows MSI
- `*.exe` — installateur Windows NSIS
- `*.nsis.zip` + `*.sig` — bundle consommé par l'updater Tauri (Windows)
- `latest.json` — manifest d'auto-update servi via `releases/latest/download/latest.json`

## Premier lancement macOS

L'app est signée Tauri (suffisant pour l'auto-update) mais pas notarized
Apple. Clic-droit sur l'icône → **Ouvrir** → confirmer.

## Auto-update

À partir de la v0.2.0 de La Fabrik, l'app vérifie automatiquement les mises à
jour au démarrage et propose un bouton manuel dans **Réglages → À propos**.
