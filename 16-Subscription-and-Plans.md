# 16 — Planes y Suscripciones

## Objetivo

Los planes son una herramienta comercial y deben ser configurables desde administración.

No se recomienda codificar los planes como reglas rígidas dentro de la aplicación.

## Componentes

Un plan puede definir:

- precio base;
- moneda;
- periodicidad;
- descuento;
- productos máximos;
- fotografías máximas;
- sucursales;
- usuarios;
- almacenamiento;
- dominio;
- módulos;
- soporte.

## Periodicidades

- mensual;
- trimestral;
- semestral;
- anual.

## Descuentos

El administrador podrá definir descuentos por período.

Ejemplo conceptual:

```text
Mensual      → precio estándar
Trimestral   → precio + descuento opcional
Semestral    → precio + descuento opcional
Anual        → precio + descuento opcional
```

## Suscripción

Estados:

- Trial;
- Active;
- Past Due;
- Suspended;
- Cancelled;
- Expired.

## Renovación

El sistema debe registrar:

- fecha de inicio;
- período;
- próxima renovación;
- pagos;
- descuentos;
- cambios de plan.

## Cambios de plan

Debe contemplarse:

- upgrade;
- downgrade;
- prorrateo futuro;
- aplicación al siguiente período.

La política comercial concreta puede definirse posteriormente.

## Add-ons

Ejemplos:

- dominio propio;
- usuarios adicionales;
- sucursales adicionales;
- almacenamiento;
- módulos premium.

## Plan Custom

Debe poder crearse una oferta específica para un cliente sin modificar código.
