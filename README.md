# Islands Dark for Zed

Порт темы Islands Dark из WebStorm 2026.2: цвета взяты из `ManyIslandsDark.theme.json` и `IslandSchemeDark.xml`.

## Установка

Zed → Extensions → **Install Dev Extension** → выбрать эту папку. Затем `theme selector: toggle` → **Islands Dark**.

## Шрифты как в WebStorm

Расширение не может задавать шрифты: это делается в `settings.json`.

1. Установи [JetBrains Mono](https://www.jetbrains.com/lp/mono/).
2. Скопируй блок из [`settings.example.jsonc`](settings.example.jsonc) в свой `settings.json`.

## Комментарии

Расширение содержит язык `comment` (форк [thedadams/zed-comment](https://github.com/thedadams/zed-comment), MIT):

- `/** */` — зелёные, `//` и `/* */` — серые, как в WebStorm;
- `TODO` / `FIXME` — салатовые.

Расширение **Comments Highlighter** (`comment`) ставить не нужно: оба регистрируют язык `comment` и будут конфликтовать.

При первой установке Zed скачает и соберёт грамматику `tree-sitter-comment`, для этого нужна сеть.
