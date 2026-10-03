# Monitor de plantas · Plant monitor

> **Estado / Status: Idea / Idea** — esto es una idea: aún no hay diseño ni código.
> this is an idea: there is no design or code yet.

[Español](#español) · [English](#english) · [Ficha en el sitio / Site page](https://oquinterol.com/es/lab/#plant-monitor)

## Español

Sensores de pH y humedad del sustrato que avisan cuando las plantas necesitan agua.

| | |
|---|---|
| **Estado** | Idea (2026-10-03) |
| **Mide** | pH · Humedad del sustrato |
| **Actúa** | Avisar cuando se requiere riego |
| **Controlador** | Por definir |
| **Enlace** | Por definir |

### Qué resolvería

Saber cuándo regar a partir de mediciones del sustrato, en lugar de hacerlo por calendario.

### Cómo lo pienso

Sensores de pH y humedad en el sustrato → lecturas periódicas → Home Assistant envía un aviso cuando hace falta agua.

### Por definir

Sensores, frecuencia de medición, umbrales y enlace de comunicación.

## English

Substrate pH and moisture sensors that send an alert when the plants need water.

| | |
|---|---|
| **Status** | Idea (2026-10-03) |
| **Measures** | pH · Substrate moisture |
| **Acts on** | Alert when watering is needed |
| **Controller** | To be decided |
| **Link** | To be decided |

### What it would solve

Knowing when to water from substrate measurements rather than a fixed schedule.

### How I think about it

pH and moisture sensors in the substrate → periodic readings → Home Assistant sends an alert when water is needed.

### To be decided

Sensors, measurement frequency, thresholds, and communication link.

## Basado en / Builds on

| Proyecto / Project | Licencia / Licence | Para qué / What for |
|---|---|---|
| _Aún ninguno / None yet_ | | |

Ver / See [`REUSING.md`](../../REUSING.md).

## Estructura / Layout

| Carpeta / Folder | Contenido / Contents | Licencia / Licence |
|---|---|---|
| `hardware/` | Esquemas, PCB, piezas 3D, lista de materiales / Schematics, PCB, 3D parts, BOM | CERN-OHL-P-2.0 |
| `firmware/` | Código del microcontrolador / Microcontroller code | MIT |
| `docs/` | Documentación, protocolos, fotos / Documentation, protocols, photos | CC BY 4.0 |
| `data/` | Mediciones y su descripción / Measurements and their description | CC BY 4.0 |
