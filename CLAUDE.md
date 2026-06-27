# CLAUDE.md — Contexto del proyecto usa-2026

## Sitio
El sitio se sirve desde la rama `main`. Todo cambio que deba verse reflejado en el sitio tiene que mergearse a `main` antes de reportarlo como listo.

## Sesiones múltiples
El usuario trabaja desde distintos dispositivos (PC y móvil). Puede haber cambios recientes en `main` hechos en otra sesión que esta sesión no conoce. Antes de modificar cualquier archivo, hacer `git pull origin main` para tener el estado actual. Si el usuario dice "ya está hecho", verificar en el repo antes de asumir que está pendiente.

## Rama de trabajo
Las ramas de feature (`claude/...`) son solo para desarrollo. El destino final siempre es `main`. Si hay conflictos al mergear, priorizar siempre la versión de `main` (más actualizada) y agregar encima solo lo nuevo.

## Archivos clave
- `pendientes.md` — checklist en markdown, fuente de verdad de tareas pre-viaje
- `index.html` — dashboard HTML principal con la misma info en formato visual (sección `#pendientes`)
- Ambos archivos deben mantenerse sincronizados cuando se agrega o tacha un pendiente

## Idioma
Todo el contenido del proyecto está en español. Las respuestas al usuario también en español.
