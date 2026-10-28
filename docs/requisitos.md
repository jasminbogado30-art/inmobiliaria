# Requisitos del MVP

Sistema web para una inmobiliaria: catálogo público de propiedades y
panel de administración para el personal.

## Requisitos funcionales

| Código | Requisito |
|---|---|
| RF-01 | Ver el listado de propiedades disponibles, paginado |
| RF-02 | Filtrar por tipo, zona y rango de precio |
| RF-03 | Ver el detalle de una propiedad con su galería de fotos |
| RF-04 | Enviar una consulta sobre una propiedad |
| RF-05 | Solicitar una visita proponiendo día y horario |
| RF-06 | Las propiedades vendidas no aparecen en el listado y su enlace directo informa que ya no están disponibles. Las reservadas se muestran con etiqueta |
| RF-07 | Iniciar sesión en el panel (administrador o agente) |
| RF-08 | Crear, editar y dar de baja propiedades, según el rol |
| RF-09 | Subir, ordenar y eliminar fotos, y elegir la principal |
| RF-10 | Cambiar el estado de una propiedad |
| RF-11 | Ver consultas y solicitudes de visita, y marcarlas como atendidas, según el rol |
| RF-12 | El administrador crea y desactiva usuarios del panel |

## Requisitos no funcionales

- La API es independiente del frontend y la consumen web y móvil.
- El modelo de usuarios prevé el rol Cliente para la fase 2.
- La autorización se valida en el servidor, por rol y por recurso.
- Los datos que llegan se validan siempre en el servidor.
- Ningún secreto (contraseñas, cadenas de conexión) se sube al repositorio.

## Fuera del MVP (fase 2)

- App móvil con cuentas de cliente, favoritos y notificaciones.
- Agenda de visitas con disponibilidad del agente.
