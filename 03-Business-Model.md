# 03 — Modelo de Negocio e Ingresos

## Fuentes principales

### 1. Suscripción de la tienda

Cada tienda paga un fee por utilizar VSH.

El precio dependerá del plan y de las capacidades contratadas.

### 2. Entrega

El cliente final paga el costo de envío asociado al pedido.

La plataforma debe permitir configurar reglas de tarifa, por ejemplo:

- tarifa fija;
- tarifa por zona;
- tarifa por distancia;
- tarifa por rango de pedido;
- envío gratis bajo determinadas condiciones;
- tarifa promocional.

## Planes comerciales dinámicos

Los planes no deben estar rígidamente programados.

El administrador global debe poder crear planes y definir:

- nombre;
- descripción;
- precio;
- límites;
- módulos habilitados;
- cantidad de productos;
- cantidad de fotografías por producto;
- número de sucursales;
- número de usuarios;
- dominio incluido;
- almacenamiento;
- funcionalidades premium;
- soporte;
- promociones.

También debe poder definir períodos:

- mensual;
- trimestral;
- semestral;
- anual.

Cada período puede tener un precio diferente y opcionalmente un descuento.

## Ejemplo de estructura comercial

### Plan Starter

- Inventario limitado.
- Hasta 5 fotografías por producto.
- URL `nombre-tienda.vsh.do`.
- Funciones básicas de pedidos.
- Una sucursal.
- Usuarios limitados.

### Plan Business

- Inventario ampliado o ilimitado.
- Hasta 20 fotografías por producto.
- Más sucursales.
- Más usuarios.
- Reportes ampliados.
- Herramientas promocionales.

### Plan Custom

Configuración individual según necesidades del comercio.

Puede incluir:

- dominio propio;
- límites personalizados;
- usuarios adicionales;
- almacenamiento adicional;
- módulos premium;
- condiciones comerciales especiales.

Los nombres y precios anteriores son ejemplos. El sistema debe permitir modificarlos sin intervención del equipo de desarrollo.

## Estrategia comercial futura

Podrán existir complementos:

- dominio personalizado;
- usuarios adicionales;
- sucursales adicionales;
- almacenamiento adicional;
- módulos premium;
- promoción destacada;
- integración con sistemas externos;
- servicios empresariales.

La plataforma debe separar **plan base** de **add-ons**, para evitar tener que crear un plan completamente nuevo por cada necesidad comercial.