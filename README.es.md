> Machine-translated from [README.md](README.md) into Español — corrections welcome.

# KimiVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KimiVibe_en.png" alt="Captura de pantalla de KimiVibe" width="auto" />
</div>

<p align="right">
  <a href="https://deepvibe.eu/kimivibe">kimivibe.eu</a>
</p>

KimiVibe es la **build de Kimi** de la familia *Vibe* — un fork de ZCode enfocado en un único proveedor: **Kimi** (Moonshot AI). Un modelo, un espacio de trabajo, un compañero — no un agente.

La familia *Vibe* distribuye una aplicación enfocada por proveedor (DeepVibe para DeepSeek, KimiVibe para Kimi, LamaVibe para Ollama, MiniVibe para MiniMax, KlausVibe para Claude, …), cada una con su propio carácter. Existe **junto a** ZCode, no en su lugar: ZCode para el flujo de trabajo multiproveedor, las aplicaciones Vibe para quienes quieren un modelo, un espacio de trabajo, un compañero. Consulta el repositorio de código fuente principal para ver el código completo.

## Descargas

Los instaladores para macOS, Windows y Linux se publican en [Releases](../../releases). El actualizador integrado comprueba este repositorio.

## Compilar desde el código fuente

Requiere Git, Node.js **24.14.0** y pnpm **10.33.2** (ver `mise.toml`).

```bash
pnpm bootstrap
# run the KimiVibe flavor in dev
pnpm dev:desktop:kimi
# package (KimiVibe flavor)
ZCODE_KIMI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Licencia y atribución

Construido sobre ZCode (Apache-2.0); la licencia y el NOTICE se conservan. KimiVibe es un proyecto independiente y no está afiliado a ZCode/Z.ai, Kimi/Moonshot ni a sus respectivos propietarios. Kimi es una marca registrada de su propietario; el logotipo se utiliza con el permiso del operador.
