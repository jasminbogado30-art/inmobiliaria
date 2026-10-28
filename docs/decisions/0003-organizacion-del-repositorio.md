# ADR 0003: Organización del repositorio

**Estado:** Aceptada · **Fecha:** 27/10/2026

## Contexto
El sistema tiene API, web, app móvil (fase 2) y documentación. Se
desarrolla en solitario y debe poder revisarse con un único enlace.

## Opciones consideradas
- A. Un solo repositorio con una carpeta por parte.
- B. Un repositorio por cada parte.
- C. Mixto: API y web juntas, móvil y documentación aparte.

## Decisión
Un solo repositorio (A), con las carpetas api/, web/, mobile/ y docs/.
La separación de responsabilidades se mantiene con carpetas, cada una
con su propio README.

## Consecuencias
- Los cambios que atraviesan varias partes se registran en un commit.
- Una sola configuración de integración continua.
- Si el sistema creciera a varios equipos, podría dividirse más adelante.
