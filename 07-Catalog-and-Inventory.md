# 07 — Catálogo e Inventario

## Catálogo

La plataforma debe soportar:

- productos;
- categorías;
- subcategorías;
- marcas;
- SKU;
- códigos de barras;
- descripciones;
- precios;
- precios promocionales;
- imágenes;
- variantes;
- atributos;
- estado de publicación.

## Fotografías

La cantidad máxima puede depender del plan.

Ejemplos:

- Starter: hasta 5;
- Business: hasta 20;
- Custom: límite configurable.

## Inventario

El inventario pertenece a la tienda y puede distribuirse por sucursal.

```text
Producto
└── Sucursal A: 15
└── Sucursal B: 8
└── Sucursal C: 23
```

## Movimientos

Cada ajuste importante debería generar un movimiento auditable:

- entrada;
- salida;
- ajuste;
- devolución;
- reserva;
- venta;
- transferencia.

## Reservas

Cuando un pedido es confirmado, el sistema debe reservar stock para reducir el riesgo de vender unidades inexistentes.

## Transferencias

En una fase posterior:

`Sucursal A → Sucursal B`

con trazabilidad completa.

## Productos futuros

La arquitectura puede evolucionar para soportar:

- combos;
- productos digitales;
- productos bajo pedido;
- productos con peso;
- seriales;
- lotes;
- fechas de vencimiento.
