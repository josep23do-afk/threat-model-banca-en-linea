# Modelo de amenazas — Banca en Línea (SBL)

Repositorio del modelo de amenazas elaborado con **OWASP Threat Dragon v2** para la Tarea 2 del curso Seguridad en Aplicaciones (093-013). Caso académico sobre una entidad bancaria ficticia.

## Contenido

| Ruta | Descripción |
|---|---|
| `modelo/TM_BancaEnLinea.json` | Proyecto Threat Dragon (formato v2): DFD Nivel 0, 1, 2A y 2B con 49 amenazas STRIDE |
| `diagramas/DFD_*.png` / `.svg` | Diagramas exportados desde Threat Dragon (Export → PNG / SVG) |
| `reportes/Reporte_ThreatDragon.pdf` | Reporte generado por Threat Dragon (Report → Print) |
| `CHANGELOG.md` | Historial de versiones del modelo |

## Cómo abrir el modelo

1. Abrir Threat Dragon (escritorio o web, v2.x).
2. *Login to Local Session* (web) o iniciar la app de escritorio.
3. **Open an existing threat model** → seleccionar `modelo/TM_BancaEnLinea.json` (o *Import* y pegar el contenido).
4. Abrir cada diagrama desde la vista del modelo; seleccionar un elemento para ver sus amenazas en el panel *Threats*.

## Convenciones

- Elementos y flujos en **rojo**: tienen amenazas abiertas.
- Título de cada amenaza: `T-xx` + nombre, igual que en el informe y la matriz de riesgos.
- Severidad Threat Dragon = nivel de riesgo inherente (P × I): Critical ≥ 20, High 12–19, Medium 6–11, Low ≤ 5.
- El campo *Mitigation* incluye control preventivo, detectivo, correctivo, tratamiento, iniciativa del roadmap, responsable y fecha objetivo.

## Versionado

Cada versión del modelo es un commit con etiqueta (`git tag`): `v0.1` … `v1.0`. Ver `CHANGELOG.md`.
Para mantenerlo como artefacto del SSDLC: cualquier cambio de arquitectura debe actualizar el DFD y las amenazas en una nueva versión revisada.
