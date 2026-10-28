# ADR 0004: Idioma del proyecto

**Estado:** Aceptada · **Fecha:** 27/10/2026

## Contexto
El proyecto es una pieza de portfolio para postularse a vacantes de IT en
empresas del país. Las herramientas, los lenguajes y la documentación
técnica del sector están en inglés, y el código elegido en la primera
línea es difícil de renombrar más adelante.

## Opciones consideradas
- A. Todo en español.
- B. Todo en inglés.
- C. Mixto, con un criterio por tipo de contenido.

## Decisión
Opción C:

| Contenido | Idioma |
|---|---|
| README | Español, con un resumen en inglés al comienzo |
| ADRs y requisitos | Español |
| Mensajes de commit | Español |
| Código (clases, métodos, tablas, columnas, rutas de la API) | Inglés |
| Textos que ve el usuario en la web | Español |

Los términos del dominio se traducen según el glosario (docs/glosario.md).

## Justificación
El código en inglés es coherente con el vocabulario del framework y con la
convención de la industria, y lo puede leer cualquier equipo. La
documentación se mantiene en español porque sus lectores son el cliente y
los reclutadores locales.

## Consecuencias
- Hay que mantener el glosario al día cuando aparezcan términos nuevos.
- Los documentos anteriores (ADR 0001 a 0003) ya estaban en español y no
  cambian.
