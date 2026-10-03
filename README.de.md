> Machine-translated from [README.md](README.md) into Deutsch — corrections welcome.

# KimiVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KimiVibe_en.png" alt="KimiVibe Screenshot" width="auto" />
</div>

<p align="right">
  <a href="https://deepvibe.eu/kimivibe">kimivibe.eu</a>
</p>

KimiVibe ist der **Kimi-Build** der *Vibe*-Familie — ein Fork von ZCode, der sich auf einen einzigen Anbieter konzentriert: **Kimi** (Moonshot AI). Ein Modell, ein Arbeitsbereich, ein Partner — kein Agent.

Die *Vibe*-Familie liefert eine fokussierte App pro Anbieter (DeepVibe für DeepSeek, KimiVibe für Kimi, LamaVibe für Ollama, MiniVibe für MiniMax, KlausVibe für Claude, …), jede mit ihrem eigenen Charakter. Sie existiert **neben** ZCode, nicht an dessen Stelle: ZCode für den Multi-Provider-Workflow, die Vibe-Apps für Menschen, die ein Modell, einen Arbeitsbereich, einen Partner wollen. Den vollständigen Codebestand findest du im Hauptquellcode-Repository.

## Downloads

Installer für macOS, Windows und Linux werden unter [Releases](../../releases) veröffentlicht. Der integrierte Updater prüft dieses Repository.

## Aus dem Quellcode bauen

Erfordert Git, Node.js **24.14.0** und pnpm **10.33.2** (siehe `mise.toml`).

```bash
pnpm bootstrap
# run the KimiVibe flavor in dev
pnpm dev:desktop:kimi
# package (KimiVibe flavor)
ZCODE_KIMI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Lizenz & Namensnennung

Basiert auf ZCode (Apache-2.0); die Lizenz und der NOTICE-Hinweis bleiben erhalten. KimiVibe ist ein unabhängiges Projekt und steht in keiner Verbindung zu ZCode/Z.ai, Kimi/Moonshot oder deren jeweiligen Eigentümern. Kimi ist eine Marke ihres Eigentümers; das Logo wird mit Erlaubnis des Betreibers verwendet.
