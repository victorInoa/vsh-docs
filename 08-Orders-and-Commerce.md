# 08 — Pedidos y Comercio

## Flujo principal

```text
Cliente
  ↓
Carrito
  ↓
Checkout
  ↓
Método de pago
  ↓
Pedido
  ↓
Confirmación
  ↓
Preparación
  ↓
Recogida
  ↓
Entrega
```

## Estados sugeridos

- Pending;
- Payment Pending;
- Confirmed;
- Preparing;
- Ready for Pickup;
- Pickup Assigned;
- Picked Up;
- Out for Delivery;
- Delivered;
- Cancelled;
- Failed;
- Returned.

## Checkout

El cliente seleccionará:

- productos;
- cantidades;
- dirección;
- método de pago;
- información de contacto;
- instrucciones de entrega.

## Métodos de pago

La plataforma debe permitir seleccionar un método por pedido, entre opciones habilitadas:

- tarjeta;
- transferencia bancaria;
- pago contra entrega;
- otros proveedores integrados.

La arquitectura debe utilizar una capa de abstracción para poder conectar diferentes gateways sin cambiar el flujo principal.

## Historial

El pedido debe conservar una fotografía histórica de la operación:

- productos;
- cantidades;
- precios;
- descuentos;
- impuestos si aplican;
- envío;
- total;
- dirección;
- método de pago.

Los cambios posteriores en catálogo o precios no deben alterar pedidos históricos.

## Devoluciones e incidencias

Debe contemplarse un módulo posterior para:

- devolución;
- producto incorrecto;
- producto faltante;
- pedido rechazado;
- entrega fallida;
- reembolso.
