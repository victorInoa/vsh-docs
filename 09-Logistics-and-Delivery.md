# 09 — Logística y Entregas

## Modelo inicial

La compañía tendrá repartidores propios disponibles para las tiendas afiliadas.

Flujo:

```text
Cliente realiza pedido
        ↓
VSH recibe pedido
        ↓
Tienda prepara pedido
        ↓
VSH coordina recogida
        ↓
Repartidor recoge
        ↓
Repartidor transporta
        ↓
Cliente recibe
        ↓
Prueba de entrega
```

## Gestión de repartidores

El sistema debe administrar:

- perfil;
- estado;
- disponibilidad;
- zona;
- vehículo;
- pedidos asignados;
- historial;
- incidencias.

Estados sugeridos:

- Offline;
- Available;
- Assigned;
- Picking Up;
- Delivering;
- Completed;
- Suspended.

## Asignación

Inicialmente puede realizarse manualmente desde un Dispatcher.

Posteriormente puede evolucionar hacia asignación automática considerando:

- distancia;
- zona;
- disponibilidad;
- carga de trabajo;
- capacidad;
- prioridad.

## Seguimiento

Futuras capacidades:

- GPS;
- ubicación en tiempo real;
- ETA;
- mapa de recorrido;
- notificación al cliente;
- prueba fotográfica;
- firma;
- código OTP.

## Integración con terceros

Aunque el modelo inicial usa repartidores propios, la arquitectura debe permitir integrar:

- empresas de delivery;
- repartidores independientes;
- flotas externas;
- APIs logísticas.

## Tarifación

El costo de entrega puede configurarse por:

- zona;
- distancia;
- horario;
- tipo de servicio;
- peso/volumen;
- condiciones promocionales.

El fee de envío será cobrado al cliente final.

## Incidencias

Debe existir trazabilidad de:

- cliente ausente;
- dirección incorrecta;
- tienda cerrada;
- producto no disponible;
- vehículo averiado;
- rechazo;
- devolución.
