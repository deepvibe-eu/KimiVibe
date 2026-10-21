> Machine-translated from [README.md](README.md) into Español — corrections welcome.

# KimiVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KimiVibe_en.png" alt="Captura de pantalla de KimiVibe" width="auto" />
</div>

<p align="right">
  <a href="https://deepvibe.eu/kimivibe">kimivibe.eu</a>
</p>

KimiVibe es la **build de Kimi** de la familia *Vibe* — un fork de ZCode centrado en un único proveedor: **Kimi** (Moonshot AI). Un modelo, un espacio de trabajo, un compañero — no un agente.

La familia *Vibe* distribuye una aplicación enfocada por proveedor (DeepVibe para DeepSeek, KimiVibe para Kimi, LamaVibe para Ollama, MiniVibe para MiniMax, KlausVibe para Claude, …), cada una con su propio carácter. Existe **junto a** ZCode, no en su lugar: ZCode para el flujo de trabajo multiproveedor, las aplicaciones Vibe para quienes quieren un modelo, un espacio de trabajo, un compañero. Consulta el repositorio principal del código fuente para ver el código completo.

## Descargas

Los instaladores para macOS, Windows y Linux están en la [página de releases](../../releases); la versión más reciente siempre lleva la etiqueta **latest**:

| Plataforma | Archivos |
| --- | --- |
| macOS (Apple Silicon) | `KimiVibe-<version>-mac-arm64.dmg` · `KimiVibe-<version>-mac-arm64.zip` |
| Windows | `KimiVibe-<version>-win-x64.exe` |
| Linux | `KimiVibe-<version>-linux-x86_64.AppImage` · `KimiVibe-<version>-linux-amd64.deb` · `KimiVibe-<version>-linux-x86_64.rpm` · `KimiVibe-<version>-linux-x64.pkg.tar.zst` |

Todas las aplicaciones de la familia *Vibe* se publican con el **mismo número de versión** (actualmente 1.0.5). El actualizador integrado comprueba la última release de este repositorio.

> **macOS (Apple Silicon):** la build **no está firmada** (sin Apple Developer Program de pago), por lo que Gatekeeper
> muestra una advertencia en el primer arranque. La aplicación está firmada de forma ad-hoc — ábrela una vez mediante **clic derecho → Abrir**, o ejecuta
> `xattr -dr com.apple.quarantine "/Applications/KimiVibe.app"`.

## Compilar desde el código fuente

Requiere Git, Node.js **24.14.0** y pnpm **10.33.2** (consulta `mise.toml`).

```bash
pnpm bootstrap
# ejecutar la variante KimiVibe en modo desarrollo
pnpm dev:desktop:kimi
# empaquetar (variante KimiVibe)
ZCODE_KIMI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licencia y atribución

Construido sobre ZCode (Apache-2.0); la licencia y el NOTICE se conservan. KimiVibe es un proyecto independiente y no está afiliado a ZCode/Z.ai, Kimi/Moonshot ni a sus respectivos propietarios. Kimi es una marca registrada de su propietario; el logotipo se utiliza con el permiso del operador.
