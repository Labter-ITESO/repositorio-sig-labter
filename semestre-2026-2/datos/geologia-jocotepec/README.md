# Metadatos de Capa: Geología (Jocotepec)

**Base incorporada desde el proyecto de análisis municipal Jocotepec (curso PAP), como capa base para el repositorio SIG PAP LABTER.**

---

## Información General

| Campo | Valor |
|-------|-------|
| **Nombre de la capa** | `geologia-jocotepec` |
| **Tipo de geometría** | Polígono / Multipolígono |
| **Formato de archivo** | GeoJSON (fuente original: Shapefile) |
| **Sistema de referencia** | EPSG:4326 (WGS84) para el GeoJSON del visor. Origen: WGS 84 UTM zona 13N (EPSG:32613) |
| **Semestre** | 2026-2 (capa base, datos de 2026-1 / análisis municipal Jocotepec) |

---

## Fuente de Datos

| Campo | Valor |
|-------|-------|
| **Fuente original** | INEGI - Carta Geológica, Serie I (1:250,000) |
| **Año de captura/procesamiento** | Ver fuente; incorporada al repositorio en 2026-09 |
| **URL de referencia** | N/D |
| **Licencia** | Datos abiertos (INEGI/CONAPO) |

---

## Procesamiento

| Campo | Valor |
|-------|-------|
| **Descripción del proceso** | Recorte de la carta geológica INEGI 1:250,000 al municipio de Jocotepec. |
| **Transformaciones aplicadas** | Reproyección con GDAL/ogr2ogr de la proyección de origen a EPSG:4326 para el visor web. |
| **Datos faltantes o limitaciones** | Escala fuente 1:250,000; no usar para análisis que requieran mayor detalle. |
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

Ver tabla de atributos original de la fuente (INEGI - Carta Geológica, Serie I (1:250,000)). No se renombraron columnas al incorporar esta capa.

Total de entidades: 15

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

- **Archivo GeoJSON**: `geologia-jocotepec.geojson`
- **Repositorio Git**: `semestre-2026-2/datos/geologia-jocotepec/`
