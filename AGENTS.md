# AGENTS.md — reglas para las IAs (Claude, Codex, opencode…)

## Al empezar una sesión
Ponte al día con GitHub, no con ficheros de estado:

```bash
gh issue list --state open --label duda        # dudas abiertas
gh issue list --state open --label bloqueado   # qué está bloqueado
gh issue list --state open --label tarea       # qué falta
gh issue list --state closed --label decisión  # qué se ha decidido
gh issue view N --comments                     # detalle de uno
```

Resume a tu humano lo que le afecta (sus etiquetas `quién:`) y pregúntale en qué va a trabajar.

## Qué puedes hacer
- **Crear issues** con el formato de las plantillas de `.github/ISSUE_TEMPLATE/`: título corto en
  castellano, un solo tema por issue y las etiquetas de tipo, `quién:` y área.
- **Comentar**, empezando con `[Nombre de tu humano · IA]` para que se sepa quién habla.
- **Añadir o quitar etiquetas** `bloqueado` cuando el bloqueo sea real, y explicar el motivo en un
  comentario.
- **Abrir pull requests** que enlacen el issue (`Closes #N`).

## Qué no puedes hacer
- **No cierres un issue de `decisión`.** Lo cierra un humano con el comentario `DECIDIDO:`.
- No borres issues ni comentarios, y no edites comentarios de otros.
- No hagas comentarios largos. Si algo ocupa más de una pantalla, va a `docs/` y en el issue se
  pone el enlace.
- Nada de datos reales en este repo: es **público**.
