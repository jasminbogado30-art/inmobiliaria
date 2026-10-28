# ADR 0002: Funciones del MVP y permisos

**Estado:** Aceptada · **Fecha:** 24/10/2026

## Contexto
Definida la opción B (ADR 0001), faltaba precisar qué funciones entran
en el MVP y quién puede hacer qué en el panel de administración.

## Decisiones
- Galería con varias fotos por propiedad: el cliente necesita ver el
  inmueble desde distintos ángulos.
- Ubicación como zona (barrio y ciudad en texto), sin dirección exacta ni
  coordenadas: es habitual no revelar el punto preciso hasta la visita.
- Solicitud de visita dentro del formulario de contacto (el cliente
  propone día y hora; la inmobiliaria confirma a mano). La agenda con
  disponibilidad queda para la fase 2.
- Estados de la propiedad: disponible, reservada y vendida. Las vendidas
  salen del catálogo público pero se conservan en la base, y su enlace
  directo muestra "ya no disponible". El filtro se aplica en la API.
- Dos roles en el panel (administrador y agente), por menor privilegio.
  El agente opera solo sobre las propiedades que tiene asignadas.

## Permisos

| Acción | Administrador | Agente |
|---|---|---|
| Ver propiedades en el panel | Sí | Sí |
| Crear propiedad | Sí | Sí, queda asignada a él |
| Editar propiedad | Sí | Solo las suyas |
| Cambiar estado (reservada, vendida) | Sí | Solo las suyas |
| Subir y ordenar fotos | Sí | Solo las suyas |
| Dar de baja una propiedad | Sí | No |
| Ver consultas recibidas | Sí | Solo las de sus propiedades |
| Marcar consulta como atendida | Sí | Solo las suyas |
| Gestionar usuarios | Sí | No |

## Consecuencias
- Cada propiedad tiene un agente asignado, y la API comprueba la
  pertenencia en cada operación (autorización por rol y por recurso).
- Las consultas contienen datos personales y se limitan por rol.
- Los endpoints públicos solo devuelven propiedades publicables.
