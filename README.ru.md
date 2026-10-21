> Machine-translated from [README.md](README.md) into Русский — corrections welcome.

# KimiVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KimiVibe_en.png" alt="Скриншот KimiVibe" width="auto" />
</div>

<p align="right">
  <a href="https://deepvibe.eu/kimivibe">kimivibe.eu</a>
</p>

KimiVibe — это **сборка Kimi** из семейства *Vibe* — форк ZCode, ориентированный на одного провайдера: **Kimi** (Moonshot AI). Одна модель, одно рабочее пространство, партнёр — а не агент.

Семейство *Vibe* выпускает по одному специализированному приложению на каждого провайдера (DeepVibe для DeepSeek, KimiVibe для Kimi, LamaVibe для Ollama, MiniVibe для MiniMax, KlausVibe для Claude, …), каждое со своим характером. Оно существует **наряду** с ZCode, а не вместо него: ZCode — для работы с несколькими провайдерами, приложения Vibe — для тех, кому нужна одна модель, одно рабочее пространство, один партнёр. Полный исходный код смотрите в основном репозитории.

## Загрузки

Установщики для macOS, Windows и Linux доступны на [странице релизов](../../releases); самый новый релиз всегда помечен тегом **latest**:

| Платформа | Файлы |
| --- | --- |
| macOS (Apple Silicon) | `KimiVibe-<version>-mac-arm64.dmg` · `KimiVibe-<version>-mac-arm64.zip` |
| Windows | `KimiVibe-<version>-win-x64.exe` |
| Linux | `KimiVibe-<version>-linux-x86_64.AppImage` · `KimiVibe-<version>-linux-amd64.deb` · `KimiVibe-<version>-linux-x86_64.rpm` · `KimiVibe-<version>-linux-x64.pkg.tar.zst` |

Все приложения семейства *Vibe* выпускаются с **одинаковым номером версии** (сейчас 1.0.5). Встроенное средство обновления проверяет последний релиз этого репозитория.

> **macOS (Apple Silicon):** сборка **неподписанная** (нет платной программы Apple Developer Program), поэтому Gatekeeper
> предупреждает при первом запуске. Приложение подписано ad-hoc — откройте его один раз через **правый клик → Открыть** или выполните
> `xattr -dr com.apple.quarantine "/Applications/KimiVibe.app"`.

## Сборка из исходного кода

Требуются Git, Node.js **24.14.0** и pnpm **10.33.2** (см. `mise.toml`).

```bash
pnpm bootstrap
# запустить вариант KimiVibe в режиме разработки
pnpm dev:desktop:kimi
# упаковать (вариант KimiVibe)
ZCODE_KIMI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Лицензия и атрибуция

Создано на основе ZCode (Apache-2.0); лицензия и NOTICE сохранены. KimiVibe — независимый проект и не связан с ZCode/Z.ai, Kimi/Moonshot или их соответствующими владельцами. Kimi является товарным знаком своего владельца; логотип используется с разрешения оператора.
