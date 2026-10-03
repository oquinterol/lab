# Reutilizar otros proyectos · Reusing other projects

[Español](#español) · [English](#english)

## Español

No se trata de reinventar la rueda. Si un proyecto abierto existente sirve (firmware, librería, diseño de PCB, pieza 3D, protocolo), se integra, **con crédito a sus autores y respetando su licencia**.

### Cómo integrarlo (de preferencia a último recurso)

1. **Como dependencia**: librería de PlatformIO/Arduino, componente de ESPHome, integración de Home Assistant, paquete de Python. No se copia código; se declara la versión.
2. **Como submódulo de git** en la carpeta del proyecto (`git submodule add <url> projects/<id>/firmware/vendor/<nombre>`), fijado a un commit o etiqueta.
3. **Copiado (vendoring)** solo si hay que modificarlo: en su propia subcarpeta, con su `LICENSE` original y una nota de qué se cambió.

### Cómo dar crédito

- En el README del proyecto, sección **Basado en**: nombre, enlace, licencia y para qué se usa.
- En [`THIRD_PARTY.md`](THIRD_PARTY.md): una fila por proyecto reutilizado.
- En el sitio: campo `basedOn` de la ficha en `oquinterol/oquinterol` (`src/content/lab/{es,en}/<id>.md`).
- Nunca borrar avisos de copyright ni archivos `LICENSE`/`NOTICE` del original.

### Compatibilidad con las licencias de este repositorio

| Licencia del proyecto que se reutiliza | Código (aquí MIT) | Hardware (aquí CERN-OHL-P-2.0) | Docs y datos (aquí CC BY 4.0) |
|---|---|---|---|
| MIT, BSD, ISC, Apache-2.0 | ✅ Conservar su aviso (Apache: también `NOTICE`) | — | — |
| LGPL / GPL | ⚠️ Usable, pero el firmware que la incluye se distribuye **bajo GPL**; mantenerla en su carpeta y declarar la licencia resultante | — | — |
| CERN-OHL-P, licencias permisivas de hardware | — | ✅ Conservar avisos | — |
| CERN-OHL-W | — | ⚠️ Las modificaciones a esa parte siguen bajo CERN-OHL-W | — |
| CERN-OHL-S, TAPR OHL, GPL para hardware | — | ⚠️ El diseño derivado queda **bajo esa licencia recíproca**; declararlo en el proyecto | — |
| CC0, CC BY | — | — | ✅ Atribuir |
| CC BY-SA | — | — | ⚠️ Lo derivado se publica bajo CC BY-SA |
| CC BY-NC, CC BY-ND, «solo uso personal» | ❌ No son licencias abiertas: enlazar, no incluir | ❌ | ❌ |
| Sin licencia | ❌ Todos los derechos reservados: enlazar o pedir permiso al autor | ❌ | ❌ |

Si una dependencia cambia la licencia efectiva de un proyecto (p. ej. firmware GPL), se indica en el README de ese proyecto. La licencia del resto del repositorio no cambia.

> Esta tabla es una guía práctica, no asesoría legal.

## English

No reinventing the wheel. When an existing open project fits (firmware, library, PCB design, 3D part, protocol), it is integrated, **with credit to its authors and within its licence**.

### How to integrate it (preferred first)

1. **As a dependency**: PlatformIO/Arduino library, ESPHome component, Home Assistant integration, Python package. No code is copied; the version is pinned.
2. **As a git submodule** inside the project folder (`git submodule add <url> projects/<id>/firmware/vendor/<name>`), pinned to a commit or tag.
3. **Vendored copy** only when it must be modified: in its own subfolder, with its original `LICENSE` and a note on what changed.

### How to give credit

- In the project README, **Builds on** section: name, link, licence, and what it is used for.
- In [`THIRD_PARTY.md`](THIRD_PARTY.md): one row per reused project.
- On the site: the `basedOn` field of the entry in `oquinterol/oquinterol` (`src/content/lab/{es,en}/<id>.md`).
- Never remove copyright notices or upstream `LICENSE`/`NOTICE` files.

### Compatibility with this repository's licences

| Licence of the reused project | Code (here MIT) | Hardware (here CERN-OHL-P-2.0) | Docs and data (here CC BY 4.0) |
|---|---|---|---|
| MIT, BSD, ISC, Apache-2.0 | ✅ Keep its notice (Apache: also `NOTICE`) | — | — |
| LGPL / GPL | ⚠️ Usable, but firmware that includes it is distributed **under the GPL**; keep it in its own folder and state the resulting licence | — | — |
| CERN-OHL-P, permissive hardware licences | — | ✅ Keep notices | — |
| CERN-OHL-W | — | ⚠️ Changes to that part stay under CERN-OHL-W | — |
| CERN-OHL-S, TAPR OHL, GPL for hardware | — | ⚠️ The derived design falls **under that reciprocal licence**; state it in the project | — |
| CC0, CC BY | — | — | ✅ Attribute |
| CC BY-SA | — | — | ⚠️ Derived material is published under CC BY-SA |
| CC BY-NC, CC BY-ND, "personal use only" | ❌ Not open licences: link, don't include | ❌ | ❌ |
| No licence | ❌ All rights reserved: link or ask the author | ❌ | ❌ |

If a dependency changes a project's effective licence (e.g. GPL firmware), that project's README says so. The rest of the repository keeps its licences.

> This table is practical guidance, not legal advice.
