# Mapa de arquitectura — CRM Academia Diabetes Online

Mapa interactivo del CRM construido por Jesús Martínez para Academia Diabetes Online (Vite + React 19 + Supabase). Hecho por Horus Scale durante la evaluación de mantenimiento (mayo 2026).

**URL pública**: https://horusscale.github.io/crm-ado-architecture-map/

## Qué incluye

- ~80 nodos en 6 clusters (Entrada · Audiencias · Vistas · Services · Backend Supabase · Integraciones)
- ~80 edges etiquetados (critical, mount, api, db, internal)
- Espina dorsal del flujo de onboarding (Lead → Cliente activo) en línea roja
- Filter chips por feature: Onboarding, Ciclo semanal, Nutrición, Training, Portal cliente, Contabilidad/Renovaciones, Código muerto
- Sidebar con 12 hallazgos notables (deuda técnica concentrada, código muerto, smells)
- Pan + zoom + selección con click

## Cómo usar

Abre el HTML directamente en navegador (o sirve con `python3 -m http.server`). Click en cualquier nodo para ver detalle. Click en un chip para destacar un flujo. Arrastra para desplazar; rueda para zoom.

## Editar a mano

`index.html` es auto-contenido. Los arrays `clusters`, `nodes`, `edges` y `FINDINGS` están al inicio del `<script>` y se pueden editar a mano sin tocar el resto del código.
