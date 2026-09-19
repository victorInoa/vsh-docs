# 20 — Escalabilidad y Evolución

## Escalabilidad comercial

La plataforma debe poder incorporar nuevas tiendas sin crear una aplicación independiente.

## Escalabilidad técnica

La arquitectura debe permitir evolucionar hacia:

- colas;
- workers;
- cache;
- almacenamiento de objetos;
- CDN;
- búsqueda especializada;
- bases de datos optimizadas;
- servicios especializados.

## Escalabilidad logística

El modelo debe permitir pasar de:

```text
Pocos repartidores
```

a:

```text
Múltiples zonas
Múltiples equipos
Múltiples vehículos
Terceros logísticos
```

## Aplicaciones futuras

### App del repartidor

- disponibilidad;
- pedidos;
- navegación;
- recogida;
- entrega;
- evidencia.

### App del Owner

- ventas;
- pedidos;
- inventario;
- alertas.

### App del cliente

- compras;
- seguimiento;
- favoritos;
- promociones.

## Marketplace

Aunque no forma parte del alcance inicial, el modelo de tenants debe permitir posteriormente una capa de descubrimiento global.

## Integraciones

Posibles integraciones futuras:

- POS;
- ERP;
- contabilidad;
- facturación;
- gateways;
- mapas;
- WhatsApp;
- proveedores logísticos.

## Inteligencia operacional

A futuro se pueden introducir automatizaciones para:

- detectar bajo stock;
- sugerir reposición;
- predecir demanda;
- asignar pedidos;
- optimizar rutas.
