# Lab · Laboratorio abierto

Open hardware y open software para un laboratorio conectado: cultivo de microalgas y cianobacterias, incubación, monitoreo de plantas e instrumentación, todo reportando a un sistema central en Home Assistant.
*Open hardware and open software for a connected lab — culturing, incubation, plant monitoring, and instrumentation, all reporting to a central Home Assistant system.*

**Sitio / Site:** [oquinterol.com/es/lab](https://oquinterol.com/es/lab/) · [oquinterol.com/en/lab](https://oquinterol.com/en/lab/)

[Español](#español) · [English](#english)

## Español

Este repositorio es un cuaderno de laboratorio público. Cada proyecto declara su estado real (`idea → prototipo → experimental → activo → completado`); lo que todavía es idea se presenta como idea, no como un sistema construido.

### Arquitectura

```
dispositivos ──LoRa──▶ gateway LoRa ──▶ Home Assistant ──▶ automatizaciones y alertas
             └─Wi-Fi──────────────────▶
```

Los dispositivos de bajo consumo transmiten por LoRa para no congestionar el Wi-Fi.

### Proyectos

| Proyecto | Estado |
|---|---|
| [Fotobiorreactor con luz regulada](projects/photobioreactor/) | Idea |
| [Incubadora con agitación controlada](projects/shaking-incubator/) | Idea |
| [Monitor de plantas](projects/plant-monitor/) | Idea |
| [Termociclador conectado](projects/connected-thermocycler/) | Idea |
| [Cuantificador de ADN conectado](projects/connected-dna-quantifier/) | Idea |
| [Cabina de flujo conectada](projects/connected-flow-hood/) | Idea |

### Compartido

- [`shared/gateway-lora/`](shared/gateway-lora/) — gateway LoRa
- [`shared/home-assistant/`](shared/home-assistant/) — integración y automatizaciones
- [`shared/data-format/`](shared/data-format/) — formato común de mediciones

## English

This repository is a public lab notebook. Each project states its real status (`idea → prototype → experimental → active → completed`); what is still an idea is presented as an idea, not as a built system.

### Architecture

```
devices ──LoRa──▶ LoRa gateway ──▶ Home Assistant ──▶ automations and alerts
        └─Wi-Fi──────────────────▶
```

Low-power devices transmit over LoRa to keep Wi-Fi uncongested.

### Projects

| Project | Status |
|---|---|
| [Light-regulated photobioreactor](projects/photobioreactor/) | Idea |
| [Controlled shaking incubator](projects/shaking-incubator/) | Idea |
| [Plant monitor](projects/plant-monitor/) | Idea |
| [Connected thermocycler](projects/connected-thermocycler/) | Idea |
| [Connected DNA quantifier](projects/connected-dna-quantifier/) | Idea |
| [Connected flow hood](projects/connected-flow-hood/) | Idea |

## Licencias / Licences

| Qué / What | Licencia / Licence | Archivo / File |
|---|---|---|
| Hardware (esquemas, PCB, piezas / schematics, PCB, parts) | [CERN-OHL-P-2.0](https://ohwr.org/cern_ohl_p_v2.txt) | [`LICENSE-HARDWARE`](LICENSE-HARDWARE) |
| Firmware y código / Firmware and code | [MIT](https://opensource.org/license/mit) | [`LICENSE`](LICENSE) |
| Documentación y datos / Documentation and data | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | [`LICENSE-DOCS`](LICENSE-DOCS) |

Cómo citar / How to cite: [`CITATION.cff`](CITATION.cff). Contribuir / Contributing: [`CONTRIBUTING.md`](CONTRIBUTING.md).
