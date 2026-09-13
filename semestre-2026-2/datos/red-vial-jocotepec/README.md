# Metadatos de Capa: Red vial (Jocotepec)

**Base incorporada desde el proyecto de análisis municipal Jocotepec (curso PAP), como capa base para el repositorio SIG PAP LABTER.**

---

## Información General

| Campo | Valor |
|-------|-------|
| **Nombre de la capa** | `red-vial-jocotepec` |
| **Tipo de geometría** | Línea / Multilínea (+4 GeometryCollection) |
| **Formato de archivo** | GeoJSON (fuente original: Shapefile) |
| **Sistema de referencia** | EPSG:4326 (WGS84) para el GeoJSON del visor. Origen: Sin archivo .prj en la fuente; se asumió Lambert Conformal Conic México (EPSG:6372, proyección estándar de INEGI) tras validar que así el trazado cae correctamente sobre Jocotepec. **Verificar este supuesto si se detectan desalineaciones.** |
| **Semestre** | 2026-2 (capa base, datos de 2026-1 / análisis municipal Jocotepec) |

---

## Fuente de Datos

| Campo | Valor |
|-------|-------|
| **Fuente original** | INEGI - Red Nacional de Caminos, ed. 1 (Jalisco) |
| **Año de captura/procesamiento** | Ver fuente; incorporada al repositorio en 2026-09 |
| **URL de referencia** | N/D |
| **Licencia** | Datos abiertos (INEGI/CONAPO) |

---

## Procesamiento

| Campo | Valor |
|-------|-------|
| **Descripción del proceso** | Recorte de la Red Nacional de Caminos de INEGI al municipio de Jocotepec. El shapefile de origen no traía archivo .prj; se determinó la proyección de origen por prueba (EPSG:6372) comparando contra las demás capas ya recortadas. |
| **Transformaciones aplicadas** | Reproyección con GDAL/ogr2ogr de la proyección de origen a EPSG:4326 para el visor web. |
| **Datos faltantes o limitaciones** | 4 features llegaron como GeometryCollection en vez de línea/multilínea; revisar si el visor las requiere simplificadas a MultiLineString. |
| **Precisión/Exactitud** | Heredada de la fuente original; no se realizaron ajustes de precisión. |

---

## Responsables

| Campo | Valor |
|-------|-------|
| **Autor/Estudiante** | Aldo Gil |
| **Correo de contacto** | aldo.jgp@gmail.com |
| **Profesor responsable** | Aldo Gil |
| **Fecha de creación** | 2026-09 |
| **Última actualización** | 2026-09 |

---

## Atributos de la capa

Ver tabla de atributos original de la fuente (INEGI - Red Nacional de Caminos, ed. 1 (Jalisco)). No se renombraron columnas al incorporar esta capa.

Total de entidades: 1611

---

## Cambios respecto a versión anterior

Capa nueva en el repositorio (primera incorporación como capa base).

---

## Control de Calidad

- [x] Geometría validada (conversión GDAL sin errores)
- [x] Proyección verificada por comparación de bounding box contra capas hermanas del mismo análisis municipal
- [ ] Atributos completos (sin NULL innecesarios) — no revisado a detalle
- [ ] Nombres de campos estandarizados — no renombrados, se dejaron como en la fuente
- [ ] Documentación completada — completar año/escala exactos si se conocen

---

## Notas Adicionales

> Esta capa proviene del proyecto de análisis municipal de Jocotepec (curso PAP), reutilizada como capa base del repositorio SIG PAP LABTER a petición del profesor. Los campos "Fecha de captura" y "Escala" en `config.json` son inferencias a partir de los nombres de archivo de la fuente INEGI/CONAPO; revisar y ajustar si se cuenta con el dato exacto.

---

## Descargar esta capa

- **Archivo GeoJSON**: `red-vial-jocotepec.geojson`
- **Repositorio Git**: `semestre-2026-2/datos/red-vial-jocotepec/`
