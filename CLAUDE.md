# CLAUDE.md — Contexto del proyecto usa-2026

## Sitio
El sitio se sirve desde la rama `main`. Todo cambio que deba verse reflejado en el sitio tiene que mergearse a `main` antes de reportarlo como listo.

## Sesiones múltiples
El usuario trabaja desde distintos dispositivos (PC y móvil). Puede haber cambios recientes en `main` hechos en otra sesión que esta sesión no conoce. Antes de modificar cualquier archivo, hacer `git pull origin main` para tener el estado actual. Si el usuario dice "ya está hecho", verificar en el repo antes de asumir que está pendiente.

## Rama de trabajo
Las ramas de feature (`claude/...`) son solo para desarrollo. El destino final siempre es `main`. Si hay conflictos al mergear, priorizar siempre la versión de `main` (más actualizada) y agregar encima solo lo nuevo.

## Archivos clave
- `pendientes.md` — checklist en markdown, fuente de verdad de tareas pre-viaje
- `index.html` — dashboard HTML principal con la misma info en formato visual (sección `#pendientes`). Este es el ÚNICO archivo HTML que se edita y se pushea — no crear copias con otro nombre (ej. "viaje_usa_versionB.html"); eso fue la causa de que ediciones desde Mac pisaran cambios ya hechos desde el celular.
- Ambos archivos deben mantenerse sincronizados cuando se agrega o tacha un pendiente
- `links.md`, `spots.md`, `Itinerario_EEUU_Agosto2026.xlsx`, `turo_bloque2.md` y los `*-ruta.html` — documentos de respaldo/planning solo locales, no viven en el repo ni se pushean.

## Regla de oro para evitar desincronización
Esta carpeta (`~/Desktop/Proyectos activos/USA 2026/`) ES el clon git del repo (`origin/main`) — no una copia aparte. Antes de editar CUALQUIER archivo acá: `git pull origin main`. Después de editar: `git add`, `git commit`, `git push` directo desde acá. Nunca copiar este `index.html` a otra carpeta temporal para pushear — eso reintroduce el bug de trabajar con una copia vieja.

## Idioma
Todo el contenido del proyecto está en español. Las respuestas al usuario también en español.

## Estado al 5/7/2026
- **GuideAlong** — comprado y configurado. Tour "Yellowstone & Grand Teton National Parks" descargado (196 MB). Funciona con CarPlay: abrir app, tocar "Start Touring" y el GPS dispara los audios automáticamente mientras se maneja.
- **eSIM** — Holafly 23 días ilimitados USA, comprada para Daniel y Melisa.
- **Apps Daniel** — todas instaladas ✅ (Uber, Lyft, Waymo, SpotHero, ParkWhiz, ParkMobile, GuideAlong, AllTrails, Yelp, Google Translate, Apple Pay). ParkMobile sin cuenta activa — requiere SIM USA para OTP.
- **Apps Melisa** — todas instaladas ✅ (Lyft, Waymo, SpotHero, ParkWhiz, ParkMobile, Apple Wallet).
- **Ticketmaster** — instalada en ambos celulares ✅. Tickets AC/DC visibles en la app.
- **PID** — hecho, de las primeras tareas resueltas.
- **Partido Sounders vs. Querétaro (9/8, Leagues Cup, Lumen Field, gates 1 PM / kickoff 2 PM)** — DECISIÓN TOMADA: se agrega como actividad confirmada del Día 9 (no opcional), entre Seattle Center (mañana) y Capitol Hill (noche). Link de tickets en el propio `<li>` del día. Falta comprar las entradas (ver `pendientes.md`).
- **Google Maps offline / My Maps** — pendiente. Crear mapas por ciudad y parques, descargar zonas offline para CarPlay.
- **Challenger LA (Turo)** — disponibilidad incierta desde el 29/6 (accidente por otro guest, claim abierto). Turo cubre con reemplazo si no llega a tiempo.
- **Top Pot Doughnuts** (Día 8) y **Elliott Bay Book Company** (Día 9, Capitol Hill) — agregados al itinerario de Seattle.
