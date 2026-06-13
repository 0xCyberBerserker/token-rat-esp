<p align="center">
  <img src="assets/icon.png" alt="token-rat-esp icon" width="128">
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
![Not malware](https://img.shields.io/badge/Not%20malware-just%20token%20frugal-red?style=flat-square)

Spanish Codex skill for shorter answers, cleaner patches and token-efficient developer workflows.

¿Cansado de que Codex te escriba una novela para tocar tres líneas?

¿Tu output se bebe los créditos como una rata en buffet libre?

`token-rat-esp` es una skill para pedir respuestas cortas, técnicas y útiles. Menos ruido. Más patch. Cero humo.

No es un RAT. Es una rata de tokens: una skill para ahorrar output en Codex.

También funciona con Gemini por CLI como prompt de trabajo compacto.

## Qué hace

- Fuerza respuestas compactas.
- Mantiene el español como base.
- Deja los términos técnicos en inglés cuando aclaran más.
- Empuja a patches pequeños y scope mínimo.

## Para qué sirve

- Cambios de código rápidos.
- Debugging ajustado.
- Notas de review mínimas.
- Respuestas operativas cortas.

## Instalación

Copia la carpeta `token-rat-esp/` dentro de la ruta de skills de Codex.

Rutas típicas:

- `~/.codex/skills/`
- tu directorio de skills de Claude, si las espejas allí

Si trabajas con Gemini por CLI, puedes reutilizar `SKILL.md` como base instruction o prompt persistente de tu flujo.

## Integración automática

La skill ya queda preparada para auto-discovery en Codex si está instalada en `~/.codex/skills/token-rat-esp`.

Además, incluye `agents/openai.yaml` con:

- `policy.allow_implicit_invocation: true`
- `default_prompt` para sugerir su uso implícito

Eso ayuda a que Codex la tenga disponible sin invocarla siempre a mano.

Si quieres usarla casi siempre dentro de un repo concreto, añade una regla breve en `AGENTS.md`:

```md
Usa token-rat-esp por defecto para tareas de coding normales.
Responde en español técnico claro, con output mínimo útil.
Prioriza patch pequeño, prueba mínima y cero relleno.
```

Eso no sustituye la skill: la refuerza y la vuelve parte del comportamiento por defecto del proyecto.

## Cómo activarla

### UI

Usa el nombre de la skill en la petición:

```text
/skill token-rat-esp
```

### CLI

Pide el modo en texto plano:

- `modo rata`
- `tokens mínimos`
- `solo patch`
- `no expliques`
- `no seas plasta`

### Gemini CLI

Usa el contenido de `SKILL.md` como instrucción persistente o arranque de sesión, y luego trabaja en texto plano:

```text
token-rat-esp
Arregla este bug con output mínimo.
```

## Ejemplo

### UI

```text
/skill token-rat-esp
Arregla este bug y dame solo el patch mínimo.
```

### CLI

```text
token-rat-esp
Arregla este bug y dame solo el patch mínimo.
```

También vale:

```text
no seas plasta
Arregla este bug y dame solo el patch mínimo.
```

### Gemini CLI

```text
Usa token-rat-esp como regla de respuesta.
Arregla este bug y dame solo el patch mínimo.
```

Salida esperada:

```text
Hecho.

Tocado:
- `src/foo.ts`: null check corregido

Prueba:
`pnpm test foo`
```

## Estructura

```text
token-rat-esp/
├── README.md
├── SKILL.md
├── LICENSE
├── .gitignore
└── assets/
    └── icon.png
```

## También en esta caja de herramientas

¿Trabajas con Codex en Linux?

Mira `codex-ui-linux-port`: un proyecto unofficial de Linux packaging automation para Codex UI.

Está pensado para quien quiere un desktop workflow más limpio alrededor de Codex UI, con estructura package-friendly y release automation.

Herramienta distinta, misma filosofía:

Piensa menos en empaquetado. Construye más.

[Explore codex-ui-linux-port](https://github.com/0xCyberBerserker/codex-ui-linux-port)

## Créditos

Icono: PNG generado por el usuario y editado en GIMP.

## Licencia

Código y texto de este repositorio: MIT.

## Safety note

Este repositorio es público y solo contiene contenido público.
