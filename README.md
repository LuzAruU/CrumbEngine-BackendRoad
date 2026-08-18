# 🎂 CrumbEngine

Sistema para administrar un negocio de pastelería personalizada: catálogo de recetas,
gestión de pedidos por encargo, control de cupos por fecha y cálculo de costos e
inventario de insumos.

> **Estado:** 🚧 En construcción — Fase 1 (núcleo en memoria).
## ¿Qué resuelve?

Cuando hacés pastelería por encargo, el problema real no es la cocina: es
**no sobrevenderte**, **saber cuánto ganás por producto** y **no quedarte sin insumos**.
CrumbEngine modela justamente eso:

- **Constructor de pedidos:** el cliente arma su producto (tamaño, bizcochuelo, relleno,
  cobertura); el sistema valida que la combinación sea posible y calcula el precio.
- **Cupos por fecha:** limita cuántos pedidos aceptás por día para no saturar la cocina
  (clave en fechas pico: San Valentín, Día de la Madre).
- **Costos e inventario:** al confirmar un pedido, descuenta los ingredientes del stock
  y calcula el costo real frente al precio de venta.
- Y Probablemente muchas cosas mas que se se vera en el proceso!!!!!
## Roadmap del proyecto

Cada fase agrega una capa del roadmap:

| Fase | Entrega | Conceptos |
|------|---------|-----------|
| **1** | Núcleo en memoria (CLI): catálogo, pedidos, costos, cupos | Structs, slices, maps, funciones, manejo de errores |
| **2** | API REST + JSON | `net/http`, handlers, routing |
| **3** | Persistencia en base de datos | SQL, migraciones, transacciones (locks de fecha) |
| **4** | Autenticación (cliente / administrador) | JWT, hashing, middleware |
| **5** | Confirmaciones y estados por mail/Telegram | Procesos en segundo plano, concurrencia |
| **6** | Pagos + empaquetado | Mercado Pago/Stripe, Docker, tests, CI/CD |

## Stack

- **Lenguaje:** Go 1.26
- **Módulo:** `github.com/LuzAruU/CrumbEngine---BackendRoad`

## Cómo ejecutar

> Pendiente — se documentará al completar la Fase 1.

## Autora

**Luz Aruquipa** — [@LuzAruU](https://github.com/LuzAruU)
