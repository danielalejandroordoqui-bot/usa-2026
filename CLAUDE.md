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

## Estado al 28/6/2026
- **GuideAlong** — comprado y configurado. Tour "Yellowstone & Grand Teton National Parks" descargado (196 MB). Funciona con CarPlay: abrir app, tocar "Start Touring" y el GPS dispara los audios automáticamente mientras se maneja.
- **eSIM** — Holafly 23 días ilimitados USA, comprada para Daniel y Melisa.
- **Apps Daniel** — todas instaladas ✅ (Uber, Lyft, Waymo, SpotHero, ParkWhiz, ParkMobile, GuideAlong, AllTrails, Yelp, Google Translate, Apple Pay). ParkMobile sin cuenta activa — requiere SIM USA para OTP.
- **Apps Melisa** — todas instaladas ✅ (Lyft, Waymo, SpotHero, ParkWhiz, ParkMobile, Apple Wallet).
- **Ticketmaster** — instalada en ambos celulares ✅. Tickets AC/DC visibles en la app.
- **Partido Sounders vs. Querétaro (9/8, 14:00h, Lumen Field)** — decisión postergada para cuando estén en Seattle. No es partido de alta demanda, entradas disponibles last-minute es lo esperable. Link Ticketmaster guardado en el itinerario.
- **Google Maps offline / My Maps** — pendiente. Crear mapas por ciudad y parques, descargar zonas offline para CarPlay.
