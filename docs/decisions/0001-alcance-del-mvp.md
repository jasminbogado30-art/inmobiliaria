# ADR 0001: Alcance del MVP

**Estado:** Aceptada · **Fecha:** 24/10/2026

## Contexto
Una inmobiliaria necesita publicar sus propiedades en internet, recibir
consultas de clientes y poder cargar las propiedades sin depender de un
programador. Se trabaja en solitario, con entrega prevista para febrero.

## Opciones consideradas
- A. Solo catálogo público.
- B. Catálogo público + panel de administración con login.
- C. Plataforma completa (cuentas de clientes, favoritos, visitas, chat).

## Decisión
La web incluye la opción B. El módulo de clientes (favoritos y
notificaciones) se implementa en una app móvil como segunda fase, porque
las notificaciones push y la sincronización entre dispositivos son más
naturales en móvil.

## Consecuencias
- La API será independiente del frontend, para servir a web y móvil.
- El modelo de usuarios debe prever roles desde el diseño inicial.
- La app móvil queda fuera del plazo mínimo y se documenta como roadmap.
