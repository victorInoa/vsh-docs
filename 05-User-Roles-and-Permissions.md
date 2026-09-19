# 05 — Perfiles y Permisos

## Jerarquía

```text
GODADMIN
└── GLOBAL ADMIN
    └── OWNER
        ├── STORE
        │   ├── STORE ADMIN
        │   └── STORE STAFF
        └── STORE
```

La operación logística añade perfiles controlados por la compañía:

```text
GODADMIN
└── GLOBAL ADMIN
    ├── LOGISTICS MANAGER
    ├── DISPATCHER
    └── DRIVER / COURIER
```

El cliente final constituye el perfil consumidor del ecosistema.

## God Admin

Existe una única cuenta God Admin.

Debe crearse automáticamente durante el primer despliegue de la plataforma mediante un proceso de instalación seguro.

Responsabilidades:

- configuración inicial;
- administración de Global Admins;
- políticas globales;
- seguridad;
- módulos;
- planes;
- configuración de plataforma;
- recuperación administrativa.

El God Admin no debe ser una cuenta de uso cotidiano.

## Global Admin

Son administradores de la compañía.

Solo el God Admin puede crearlos y administrarlos.

Pueden gestionar múltiples tiendas y propietarios según los permisos asignados.

## Owner

Representa al dueño de uno o varios comercios.

Un Owner puede tener **N tiendas dentro de una misma cuenta**.

Puede:

- crear/configurar sus tiendas según las capacidades contratadas;
- administrar usuarios;
- asignar permisos;
- administrar catálogo;
- gestionar inventario;
- configurar sucursales;
- consultar pedidos y reportes.

## Store Admin

Administrador de una tienda particular.

El Owner decide qué módulos puede utilizar.

Cada módulo debe manejar permisos independientes:

- create;
- read;
- update;
- delete;
- list.

Esto permite crear perfiles operativos sin necesidad de programar roles nuevos.

## Store Staff

Usuario operativo con permisos limitados.

Ejemplos:

- vendedor;
- encargado de inventario;
- preparación de pedidos.

## Logistics Manager

Gestiona la operación logística de la compañía.

## Dispatcher

Coordina pedidos y asignación de repartidores.

## Driver / Courier

Gestiona las tareas de recogida y entrega asignadas.

## Cliente final

Puede:

- navegar;
- comprar;
- seleccionar método de pago;
- registrar dirección;
- consultar pedido;
- recibir notificaciones.
