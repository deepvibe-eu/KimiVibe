> Machine-translated from [README.md](README.md) into Français — corrections welcome.

# KimiVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KimiVibe_en.png" alt="Capture d'écran de KimiVibe" width="auto" />
</div>

<p align="right">
  <a href="https://deepvibe.eu/kimivibe">kimivibe.eu</a>
</p>

KimiVibe est la **version Kimi** de la famille *Vibe* — un fork de ZCode centré sur un seul fournisseur : **Kimi** (Moonshot AI). Un modèle, un espace de travail, un partenaire — pas un agent.

La famille *Vibe* propose une application dédiée par fournisseur (DeepVibe pour DeepSeek, KimiVibe pour Kimi, LamaVibe pour Ollama, MiniVibe pour MiniMax, KlausVibe pour Claude, …), chacune avec son propre caractère. Elle existe **aux côtés** de ZCode, et non à sa place : ZCode pour le flux de travail multi-fournisseurs, les applications Vibe pour ceux qui veulent un modèle, un espace de travail, un partenaire. Consultez le dépôt source principal pour l'ensemble du code.

## Téléchargements

Les installateurs pour macOS, Windows et Linux sont disponibles sur la [page des versions](../../releases) ; la version la plus récente est toujours étiquetée **latest** :

| Plateforme | Fichiers |
| --- | --- |
| macOS (Apple Silicon) | `KimiVibe-<version>-mac-arm64.dmg` · `KimiVibe-<version>-mac-arm64.zip` |
| Windows | `KimiVibe-<version>-win-x64.exe` |
| Linux | `KimiVibe-<version>-linux-x86_64.AppImage` · `KimiVibe-<version>-linux-amd64.deb` · `KimiVibe-<version>-linux-x86_64.rpm` · `KimiVibe-<version>-linux-x64.pkg.tar.zst` |

Chaque application de la famille *Vibe* est publiée avec le **même numéro de version** (actuellement 1.0.3). Le programme de mise à jour intégré vérifie la dernière version de ce dépôt.

> **macOS (Apple Silicon) :** la version est **non signée** (pas de programme Apple Developer payant), donc Gatekeeper
> affiche un avertissement au premier lancement. L'application est signée ad-hoc — ouvrez-la une fois via **clic droit → Ouvrir**, ou exécutez
> `xattr -dr com.apple.quarantine "/Applications/KimiVibe.app"`.

## Compilation depuis les sources

Nécessite Git, Node.js **24.14.0** et pnpm **10.33.2** (voir `mise.toml`).

```bash
pnpm bootstrap
# run the KimiVibe flavor in dev
pnpm dev:desktop:kimi
# package (KimiVibe flavor)
ZCODE_KIMI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licence et attribution

Basé sur ZCode (Apache-2.0) ; la licence et le NOTICE sont conservés. KimiVibe est un projet indépendant et n'est pas affilié à ZCode/Z.ai, Kimi/Moonshot ni à leurs propriétaires respectifs. Kimi est une marque de son propriétaire ; le logo est utilisé avec l'autorisation de l'exploitant.
