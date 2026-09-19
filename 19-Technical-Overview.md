# 19 — Visión Técnica

## Stack propuesto

La implementación puede utilizar:

- Laravel 13;
- Inertia 3;
- Vue 3;
- Composition API;
- Tailwind CSS 4;
- MariaDB;
- Vite.

## Arquitectura

Se recomienda separar:

- dominio;
- aplicación;
- infraestructura;
- interfaz.

El objetivo es evitar controladores excesivamente grandes y mantener reglas de negocio reutilizables.

## Módulos principales

```text
Identity & Access
Tenants / Stores
Catalog
Inventory
Branches
Orders
Payments
Subscriptions
Logistics
Notifications
Reports
Administration
Audit
```

## RBAC dinámico

Los permisos deben modelarse como datos.

Ejemplo:

```text
inventory.create
inventory.read
inventory.update
inventory.delete
inventory.list
```

Esto permite que el Owner construya perfiles personalizados.

## Integraciones

Las integraciones externas deben utilizar interfaces/adapters.

Esto permite sustituir:

- gateway de pago;
- proveedor SMS;
- proveedor WhatsApp;
- proveedor de mapas;
- proveedor logístico.

## API

Aunque el primer frontend pueda ser Inertia, se recomienda mantener servicios y casos de uso preparados para una futura API.

## Dominios

El sistema debe resolver el tenant a partir del hostname.

Esto permite:

- `tienda.vsh.do`;
- dominios personalizados.

## Observabilidad

Se recomienda contemplar:

- logs estructurados;
- métricas;
- auditoría;
- monitoreo;
- alertas;
- trazabilidad de pedidos.

## Calidad

La estrategia de desarrollo debe incluir:

- pruebas unitarias;
- pruebas de integración;
- pruebas de autorización;
- pruebas de aislamiento multi-tenant;
- pruebas end-to-end para flujos críticos.