# grouperp-d365-integrationpm

Micro-site de propuesta de José Galindo para el rol de Integration PM en un programa Group ERP / Dynamics 365 F&O (migración de datos e integración, España/Portugal).

- **Publicado en:** GitHub Pages, rama `main`, raíz del repo (`index.html`).
- **Tipo:** `oferta-freelance`.
- **Fuente de contenido:** [`src/SCHEME.md`](src/SCHEME.md) — es el único fichero que se edita a mano. Basado en `MICROSITE_TEMPLATE.en.md` v0.3.
- **Origen:** generado como borrador desde [`src/PROPUESTA_GroupERP_D365_IntegrationPM.md`](src/PROPUESTA_GroupERP_D365_IntegrationPM.md) (fuente externa del sistema TOS) mediante `propuesta_to_scheme.py`, y completado a mano.
- **Derivado:** `src/SCHEME.yaml` se genera automáticamente a partir del `.md`. No editar directamente: los cambios se pierden en la siguiente regeneración.
- **Modos de contenido usados (nuevos en v0.3):** "Qué aporto" en modo *logros* (4 logros con métrica real, no los pilares genéricos); "Arquitectura conceptual" en modo *puntos* (lista de gobierno: Workstreams/Cadence/Gates/Boundary), no diagrama de cajas ni imagen.
- **CV:** [`assets/cv-grouperp-d365-integrationpm.pdf`](assets/cv-grouperp-d365-integrationpm.pdf), enlazado desde el botón "Download CV" del hero (`botones_hero` → `destino: cv`, resuelto contra `cv_pdf`). Primer caso real que ejercita esa clave simbólica — no se usaba en `candidatura-bootcamp-ia`.

## ESTADO: borrador sin revisar (`version_documento: "0.2"`)

Este `SCHEME.md` es un borrador de validación del pipeline, no un entregable listo para enviar. Antes de publicarlo, revisa en `src/SCHEME.md`:

- `cliente_u_organizacion` — vacío: el PROPUESTA de origen no nombra al cliente.
- El H1, la cita del hero y los 4 títulos `###` de sección (Motivation/What I bring/Project/Closing) son sugerencias de posicionamiento, no copy aprobado.
- Sube `version_documento` a `"1.0"` cuando lo apruebes.

## Cómo regenerar el sitio

1. Editar `src/SCHEME.md` (si cambia el contenido, subir `version_documento` y anotar el motivo en su historial interno).
2. Ejecutar, desde el repo `microsite-toolkit`: `python3 build.py <ruta a este proyecto>` — produce `src/SCHEME.yaml` e `index.html`.
3. Revisar `index.html` localmente antes de hacer commit.
4. `git add`, `git commit`, `git push` — GitHub Pages republica automáticamente.

## Histórico

- v0.1 (2026-09-10) — generado como caso de validación real de `propuesta_to_scheme.py` y de los modos "logros"/"puntos" (v0.3 del toolkit) — primera oportunidad real y primer caso real en inglés que ejercitan el pipeline completo.
- v0.2 (2026-09-10) — añadido el CV adjunto (`cv_pdf` + botón "Download CV" en el hero).
