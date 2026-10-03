# Incubadora con agitación controlada · Controlled shaking incubator

> **Estado / Status: Idea / Idea** — esto es una idea: aún no hay diseño ni código.
> this is an idea: there is no design or code yet.

[Español](#español) · [English](#english) · [Ficha en el sitio / Site page](https://oquinterol.com/es/lab/#shaking-incubator)

## Español

Una incubadora con agitación controlada por un ESP32 e integrada con Home Assistant para automatizar su funcionamiento.

| | |
|---|---|
| **Estado** | Idea (2026-10-03) |
| **Mide** | Por definir |
| **Actúa** | Controlar la agitación |
| **Controlador** | ESP32 |
| **Enlace** | Por definir |

### Qué resolvería

Controlar la agitación de los cultivos desde un ESP32 y llevar su estado a Home Assistant, para programar y automatizar la incubación.

### Cómo lo pienso

ESP32 como controlador de la agitación, conectado al sistema central del laboratorio.

### Por definir

Variables a medir, mecanismo de agitación y enlace de comunicación.

## English

An incubator whose shaking is controlled by an ESP32 and integrated with Home Assistant to automate how it runs.

| | |
|---|---|
| **Status** | Idea (2026-10-03) |
| **Measures** | To be decided |
| **Acts on** | Control shaking |
| **Controller** | ESP32 |
| **Link** | To be decided |

### What it would solve

Control culture shaking from an ESP32 and bring its state into Home Assistant to schedule and automate incubation.

### How I think about it

An ESP32 as the shaking controller, connected to the lab's central system.

### To be decided

Variables to measure, shaking mechanism, and communication link.

## Estructura / Layout

| Carpeta / Folder | Contenido / Contents | Licencia / Licence |
|---|---|---|
| `hardware/` | Esquemas, PCB, piezas 3D, lista de materiales / Schematics, PCB, 3D parts, BOM | CERN-OHL-P-2.0 |
| `firmware/` | Código del microcontrolador / Microcontroller code | MIT |
| `docs/` | Documentación, protocolos, fotos / Documentation, protocols, photos | CC BY 4.0 |
| `data/` | Mediciones y su descripción / Measurements and their description | CC BY 4.0 |
