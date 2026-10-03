> Machine-translated from [README.md](README.md) into Русский — corrections welcome.

# KimiVibe

<div align="center">
  <img src="packages/desktop/build/README-images/KimiVibe_en.png" alt="Скриншот KimiVibe" width="auto" />
</div>

<p align="right">
  <a href="https://deepvibe.eu/kimivibe">kimivibe.eu</a>
</p>

KimiVibe — это **сборка Kimi** из семейства *Vibe* — форк ZCode, ориентированный на одного провайдера: **Kimi** (Moonshot AI). Одна модель, одно рабочее пространство, партнёр — не агент.

Семейство *Vibe* выпускает по одному специализированному приложению на каждого провайдера (DeepVibe для DeepSeek, KimiVibe для Kimi, LamaVibe для Ollama, MiniVibe для MiniMax, KlausVibe для Claude, …), каждое со своим характером. Оно существует **наряду** с ZCode, а не вместо него: ZCode — для работы с несколькими провайдерами, приложения Vibe — для тех, кому нужна одна модель, одно рабочее пространство, один партнёр. Полный исходный код смотрите в основном репозитории.

## Загрузки

Установщики для macOS, Windows и Linux публикуются в разделе [Releases](../../releases). Встроенное средство обновления проверяет этот репозиторий.

## Сборка из исходного кода

Требуются Git, Node.js **24.14.0** и pnpm **10.33.2** (см. `mise.toml`).

```bash
pnpm bootstrap
# run the KimiVibe flavor in dev
pnpm dev:desktop:kimi
# package (KimiVibe flavor)
ZCODE_KIMI_IDENTITY=1 pnpm bundle:desktop -- --os linux --arch x64
```

## Лицензия и атрибуция

Создано на основе ZCode (Apache-2.0); лицензия и NOTICE сохранены. KimiVibe — независимый проект, не связанный с ZCode/Z.ai, Kimi/Moonshot или их соответствующими владельцами. Kimi является товарным знаком своего владельца; логотип используется с разрешения оператора.
