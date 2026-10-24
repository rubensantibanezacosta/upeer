# uPeer

Repositorio raíz del proyecto. No contiene código: solo la documentación conjunta y los dos clientes como submódulos.

| Ruta | Repositorio | Rama |
|---|---|---|
| [`upper/`](upper) | [upeer-phone](https://github.com/rubensantibanezacosta/upeer-phone) | `main` |
| [`upper-desktop/`](upper-desktop) | [upeer-desktop](https://github.com/rubensantibanezacosta/upeer-desktop) | `main` |

`upper` es el cliente móvil (Expo / React Native + módulo nativo Android). `upper-desktop` es el cliente de escritorio (Electron).

## Clonar

```bash
git clone --recurse-submodules git@github.com:rubensantibanezacosta/upeer.git
```

Si ya está clonado sin submódulos:

```bash
git submodule update --init --recursive
```

Para actualizar los submódulos a sus últimas ramas:

```bash
git submodule update --remote --merge
```

## Documentación

- [`ROADMAP.md`](ROADMAP.md) — estado conjunto, fases B0–B12, contratos que deben cambiar en ambos clientes y matriz de pruebas cruzadas. Es la fuente de verdad de las decisiones que afectan a los dos clientes.
- [`AGENTS.md`](AGENTS.md) — reglas de trabajo para los agentes en este proyecto.
- Cada submódulo mantiene su propio roadmap: [`upper/roadmap.md`](upper/roadmap.md) y [`upper-desktop/Roadmap.md`](upper-desktop/Roadmap.md).

Una capacidad no se considera cerrada por funcionar en un solo cliente: si afecta a descubrimiento, ubicación, admisión o sincronización, necesita prueba con el otro cliente y evidencia en `ROADMAP.md`.

## Commits

Los cambios se commitean en el repositorio del cliente que los contiene, no aquí. Este repositorio solo registra el avance de los submódulos y los documentos de la raíz.
