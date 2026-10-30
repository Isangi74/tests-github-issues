# Prueba: organizar un proyecto con GitHub Issues

> **Repo de prueba, con datos inventados.** Sirve para ver si GitHub (issues, tablero,
> discusiones y pull requests) basta para que tres personas y sus IAs sepan en todo momento qué
> falta, qué está bloqueado y qué dudas siguen abiertas, sin tener que mantener ficheros de estado
> a mano.

## El proyecto de ejemplo: la Gran Caza del Gamusino 🦔

Tres amigos organizan la caza de gamusinos definitiva en la sierra. Los personajes son ficticios:

| Persona | Papel | Etiqueta |
|---|---|---|
| **Alba** | organiza: fechas, permisos, quién trae qué | `quién: alba` |
| **Bruno** | la parte técnica: trampas, linternas, cebo | `quién: bruno` |
| **Carla** | sale al campo, habla con los del pueblo y prueba cosas | `quién: carla` |

> Todo está publicado desde una sola cuenta. Por eso cada mensaje empieza con **[Alba]**,
> **[Bruno]** o **[Carla]**, y el responsable se indica con una etiqueta `quién:` en lugar de
> asignar la tarea a una persona. En un proyecto real cada uno usaría su usuario de GitHub y la
> asignación normal.

## Dónde mirar cada cosa

| Quiero saber… | Dónde |
|---|---|
| **qué dudas siguen abiertas** | [Issues con la etiqueta `duda`](../../issues?q=is%3Aopen+label%3Aduda) |
| **qué hemos decidido y por qué** | [Issues de decisión cerrados](../../issues?q=is%3Aclosed+label%3Adecisión) |
| **qué falta por hacer y quién lo lleva** | [Tareas abiertas](../../issues?q=is%3Aopen+label%3Atarea) o el tablero (pestaña *Projects*) |
| **qué está bloqueado** | [Etiqueta `bloqueado`](../../issues?q=is%3Aopen+label%3Abloqueado) |
| **cuánto falta para la primera salida** | [Hito "Primera salida"](../../milestones) |
| **ideas sueltas, sin compromiso** | pestaña *Discussions* |
| **documentos largos** | carpeta [`docs/`](docs/) |

## Reglas del juego

1. **Una cosa = un issue.** Cada issue es de un solo tipo: `duda`, `decisión`, `tarea` o `bloqueado`.
   Para abrirlo se usan las plantillas del botón *New issue*.
2. **Las decisiones se discuten en los comentarios** y se cierran con un comentario final que
   empieza con **DECIDIDO:** y explica qué se decidió y por qué. **Solo un humano cierra una decisión.**
3. **Las dudas se cierran cuando alguien las responde.** Si la respuesta obliga a decidir algo,
   se abre un issue de `decisión`.
4. **Los cambios en ficheros entran por pull request**, y la PR enlaza el issue que resuelve
   (`Closes #N`).
5. **Las IAs pueden leer, crear issues y comentar** usando `gh`. Ver [`AGENTS.md`](AGENTS.md).
