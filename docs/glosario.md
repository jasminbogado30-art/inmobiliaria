# Glosario y convenciones de nombres

Traducción de los términos del dominio al código, según el
[ADR 0004](decisions/0004-idioma-del-proyecto.md).

## Términos del dominio

| Español | Código | Comentario |
|---|---|---|
| Propiedad | `Property` | Inmueble publicado por la inmobiliaria |
| Tipo de propiedad | `PropertyType` | Casa, departamento, terreno, etc. |
| Zona | `Zone` | Barrio y ciudad, en texto. Sin dirección exacta |
| Precio | `Price` | |
| Foto | `Photo` | Una propiedad tiene varias; una es la principal |
| Consulta | `Inquiry` | Mensaje de un visitante sobre una propiedad |
| Solicitud de visita | `VisitRequest` | Consulta con un día y horario propuestos |
| Atendida | `Handled` | Estado de una consulta ya gestionada |
| Agente | `Agent` | Personal que gestiona sus propiedades asignadas |
| Administrador | `Admin` | Acceso total al panel |
| Cliente | `Client` | Fase 2: cuentas de clientes en la app móvil |

## Estados de una propiedad

| Español | Código |
|---|---|
| Disponible | `Available` |
| Reservada | `Reserved` |
| Vendida | `Sold` |

## Convenciones

- Clases y métodos en inglés, `PascalCase` (`Property`, `GetPropertyById`).
- Tablas en inglés y en plural (`Properties`, `Inquiries`).
- Rutas de la API en inglés y en plural (`/api/properties`).
- Los textos que ve el usuario en la web van en español.
- Si aparece un término nuevo, se agrega primero a este glosario.
