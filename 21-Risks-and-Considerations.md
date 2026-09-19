# 21 — Riesgos y Consideraciones

## Operación logística

La tecnología no elimina los retos físicos de la entrega.

Debe definirse:

- cobertura geográfica;
- horarios;
- zonas;
- tarifas;
- tiempos esperados;
- responsabilidad por pérdidas;
- política de devolución.

## Inventario

La disponibilidad depende de la precisión del inventario de cada tienda.

Se recomienda trazabilidad de movimientos y reservas.

## Pagos

Cada método tiene requisitos operativos y de conciliación diferentes.

La arquitectura debe desacoplar pagos del pedido.

## Multi-tenant

Un error de autorización puede exponer información entre tiendas.

Por eso el aislamiento debe probarse explícitamente.

## Escalabilidad

No conviene sobredimensionar el MVP, pero sí establecer límites arquitectónicos que permitan crecer.

## Seguridad

God Admin y cuentas administrativas requieren controles reforzados.

## Datos

La compañía debe definir políticas para:

- clientes;
- direcciones;
- pedidos;
- pagos;
- entregas;
- auditoría.

## Planes

Los límites comerciales deben ser configurables y auditablemente aplicados.

## Dependencia logística

La experiencia del cliente dependerá tanto del software como del desempeño de la operación de reparto.

## Recomendación de gestión

El proyecto debe desarrollarse por fases, validando primero:

1. incorporación de tiendas;
2. venta;
3. inventario;
4. pedido;
5. entrega;
6. suscripción.

Después se incorporan capacidades avanzadas.
