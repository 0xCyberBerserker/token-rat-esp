<p align="center">
  <img src="assets/icon.png" alt="token-rat-esp icon" width="96">
</p>

# token-rat-esp

[![GitHub stars](https://img.shields.io/github/stars/0xCyberBerserker/token-rat-esp?style=flat-square)](https://github.com/0xCyberBerserker/token-rat-esp/stargazers)
[![License](https://img.shields.io/github/license/0xCyberBerserker/token-rat-esp?style=flat-square)](LICENSE)
[![Last commit](https://img.shields.io/github/last-commit/0xCyberBerserker/token-rat-esp?style=flat-square)](https://github.com/0xCyberBerserker/token-rat-esp/commits/main)
![Repo size](https://img.shields.io/github/repo-size/0xCyberBerserker/token-rat-esp?style=flat-square)
![Made for Codex](https://img.shields.io/badge/Made%20for-Codex-black?style=flat-square)
![Language](https://img.shields.io/badge/Language-Spanish%20technical-blue?style=flat-square)
![Output](https://img.shields.io/badge/Output-token%20efficient-green?style=flat-square)
![KISS](https://img.shields.io/badge/KISS-approved-orange?style=flat-square)

¿Cansado de que Codex te escriba una novela para tocar tres líneas?

¿Tu output se bebe los créditos como una rata en buffet libre?

`token-rat-esp` es una skill para pedir respuestas cortas, técnicas y útiles. Menos ruido. Más patch. Cero humo.

## What it does

- Forces a compact response style.
- Keeps Spanish as the base language.
- Leaves technical terms in English when that is clearer.
- Pushes for small patches and minimal scope.

## What it is for

- Fast code edits.
- Tight debugging.
- Minimal review notes.
- Short operational answers.

## Install

Copy the `token-rat-esp/` folder into your Codex skills path.

Typical locations:

- `~/.codex/skills/`
- your Claude skill directory, if you mirror skills there

## Activate it

Use the skill name in the request:

```text
/skill token-rat-esp
```

Or ask for:

- `modo rata`
- `tokens mínimos`
- `solo patch`
- `no expliques`

## Example

```text
/skill token-rat-esp
Arregla este bug y dame solo el patch mínimo.
```

Expected style:

```text
Hecho.

Tocado:
- `src/foo.ts`: fixed null check

Prueba:
`pnpm test foo`
```

## File layout

```text
token-rat-esp/
├── README.md
├── SKILL.md
├── LICENSE
├── .gitignore
└── assets/
    └── icon.png
```

## Also from this toolbox

Working with Codex on Linux?

Take a look at `codex-ui-linux-port`: an unofficial Linux packaging automation project for Codex UI.

It is built for people who want a cleaner Linux desktop workflow around Codex UI, with package-friendly structure and release automation.

Different tool, same philosophy:

Think less about packaging. Spend more time building.

[Explore codex-ui-linux-port](https://github.com/0xCyberBerserker/codex-ui-linux-port)

## Credits

Icon: PNG asset provided by the user.

## License

Code and text in this repository are MIT.

## Safety note

This repository is public and contains only public content.
