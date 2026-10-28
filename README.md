# Inmobiliaria: catálogo web y panel de administración

> **English summary:** Web system for a real-estate agency: a public property
> catalog plus an admin panel for the staff. Portfolio project, built in the
> open. Code is written in English; documentation is written in Spanish.
> Status: design phase (no code yet).

> **Estado:** en construcción. Fase de diseño y documentación.

## Qué es

Sistema web para una inmobiliaria. Permite a los clientes explorar las
propiedades en internet y enviar consultas, y al personal de la inmobiliaria
cargar y gestionar sus propiedades sin depender de un programador.

## Funciones del MVP

- Catálogo público con filtros por tipo, zona y precio.
- Galería de fotos por propiedad.
- Consultas y solicitudes de visita desde la web.
- Panel de administración con inicio de sesión para administrador y agentes.
- Estados de la propiedad: disponible, reservada y vendida.

El detalle completo está en [docs/requisitos.md](docs/requisitos.md).

## Fases

| Fase | Alcance | Estado |
|---|---|---|
| 1 | API y web: catálogo público y panel de administración | En diseño |
| 2 | App móvil (Flutter) con cuentas de cliente, favoritos y notificaciones. Agenda de visitas con disponibilidad | Planificada |

## Tecnologías

- **Backend:** ASP.NET Core (C#).
- **Frontend, base de datos y alojamiento:** por definir. Cada elección se
  documenta como decisión de arquitectura antes de implementarse.

## Cómo se trabaja

Cada decisión de arquitectura se registra como un ADR (*Architecture Decision
Record*): el contexto, las opciones consideradas, lo que se eligió y por qué.

| ADR | Tema |
|---|---|
| [0001](docs/decisions/0001-alcance-del-mvp.md) | Alcance del MVP |
| [0002](docs/decisions/0002-funciones-del-mvp.md) | Funciones del MVP y permisos |
| [0003](docs/decisions/0003-organizacion-del-repositorio.md) | Organización del repositorio |
| [0004](docs/decisions/0004-idioma-del-proyecto.md) | Idioma del proyecto |

## Documentación

- [Requisitos](docs/requisitos.md)
- [Glosario y convenciones de nombres](docs/glosario.md)
- [Decisiones de arquitectura](docs/decisions/)

## Estructura del repositorio

```
docs/      Requisitos, glosario y decisiones de arquitectura
api/       API REST (próximamente)
web/       Frontend web (próximamente)
mobile/    App móvil, fase 2
```
