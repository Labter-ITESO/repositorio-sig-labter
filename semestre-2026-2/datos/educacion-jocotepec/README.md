# Metadatos de Capa: Educación (Jocotepec)

**Base incorporada desde el proyecto de análisis municipal Jocotepec (curso PAP), como capa base para el repositorio SIG PAP LABTER.**

---

## Información General

| Campo | Valor |
|-------|-------|
| **Nombre de la capa** | `educacion-jocotepec` |
| **Tipo de geometría** | Punto |
| **Formato de archivo** | GeoJSON (fuente original: Shapefile) |
| **Sistema de referencia** | EPSG:4326 (WGS84) para el GeoJSON del visor. Origen: WGS 84 UTM zona 13N (EPSG:32613) |
| **Semestre** | 2026-2 (capa base, datos de 2025-2 / análisis municipal Jocotepec) |

---

## Fuente de Datos

| Campo | Valor |
|-------|-------|
| **Fuente original** | INEGI - DENUE |
| **Año de captura/procesamiento** | Ver fuente; incorporada al repositorio en 2026-09 |
| **URL de referencia** | N/D |
| **Licencia** | Datos abiertos (INEGI/CONAPO) |

---

## Procesamiento

| Campo | Valor |
|-------|-------|
| **Descripción del proceso** | Extracción DENUE (corte 14/04/2026) de unidades económicas de educación en Jocotepec, con capa de cobertura a 400 m generada por separado (no incluida en este base). |
| **Transformaciones aplicadas** | Reproyección con GDAL/ogr2ogr de la proyección de origen a EPSG:4326 para el visor web. |
| **Datos faltantes o limitaciones** | Ver nota de vigencia DENUE arriba. |
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

Ver tabla de atributos original de la fuente (INEGI - DENUE). No se renombraron columnas al incorporar esta capa.

Total de entidades: 52

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

- **Archivo GeoJSON**: `educacion-jocotepec.geojson`
- **Repositorio Git**: `semestre-2026-2/datos/educacion-jocotepec/`
