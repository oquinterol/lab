# Fotobiorreactor con luz regulada · Light-regulated photobioreactor

> **Estado / Status: Idea / Idea** — esto es una idea: aún no hay diseño ni código.
> this is an idea: there is no design or code yet.

[Español](#español) · [English](#english) · [Ficha en el sitio / Site page](https://oquinterol.com/es/lab/#photobioreactor)

## Español

Un sistema para cultivar microalgas y cianobacterias como la espirulina, que mide la luz y regula los LED según lo que el cultivo necesita.

| | |
|---|---|
| **Estado** | Idea (2026-10-03) |
| **Mide** | Intensidad de luz |
| **Actúa** | Regular la emisión de los LED |
| **Controlador** | Por definir |
| **Enlace** | Por definir |

### Qué resolvería

Las microalgas y cianobacterias como la espirulina necesitan luz constante. En lugar de dejar los LED encendidos a una intensidad fija, el sistema mediría la luz que recibe el cultivo y ajustaría la emisión solo cuando haga falta.

### Cómo lo pienso

Sensor de luz → controlador → LED regulables, con las lecturas y el estado enviados a Home Assistant para registrar y automatizar.

### Por definir

Sensor, controlador, enlace de comunicación (LoRa o Wi-Fi) y criterios de regulación.

## English

A system for growing microalgae and cyanobacteria such as spirulina that measures light and drives the LEDs according to what the culture needs.

| | |
|---|---|
| **Status** | Idea (2026-10-03) |
| **Measures** | Light intensity |
| **Acts on** | Regulate LED output |
| **Controller** | To be decided |
| **Link** | To be decided |

### What it would solve

Microalgae and cyanobacteria such as spirulina need constant light. Instead of running the LEDs at a fixed intensity, the system would measure the light reaching the culture and adjust the output only when needed.

### How I think about it

Light sensor → controller → dimmable LEDs, with readings and state sent to Home Assistant for logging and automation.

### To be decided

Sensor, controller, communication link (LoRa or Wi-Fi), and regulation criteria.

## Estructura / Layout

| Carpeta / Folder | Contenido / Contents | Licencia / Licence |
|---|---|---|
| `hardware/` | Esquemas, PCB, piezas 3D, lista de materiales / Schematics, PCB, 3D parts, BOM | CERN-OHL-P-2.0 |
| `firmware/` | Código del microcontrolador / Microcontroller code | MIT |
| `docs/` | Documentación, protocolos, fotos / Documentation, protocols, photos | CC BY 4.0 |
| `data/` | Mediciones y su descripción / Measurements and their description | CC BY 4.0 |
