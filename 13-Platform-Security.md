# 13 — Seguridad

## Principios

- mínimo privilegio;
- aislamiento de tenants;
- autenticación segura;
- autorización por permisos;
- auditoría;
- protección de datos;
- validación de entradas;
- protección contra abuso.

## God Admin

La cuenta única debe recibir medidas reforzadas:

- configuración inicial segura;
- credenciales no predecibles;
- posibilidad de 2FA;
- auditoría;
- sesiones controladas.

## Permisos

La autorización debe comprobar:

1. identidad;
2. rol;
3. tenant;
4. módulo;
5. acción;
6. recurso.

## Datos

Debe evitarse la exposición de información entre tiendas.

## Archivos

Las imágenes y documentos deben almacenarse con rutas controladas y permisos apropiados.

## Auditoría

Acciones sensibles deben ser registradas.

## Disponibilidad

Se recomienda considerar:

- backups;
- monitoreo;
- logs;
- alertas;
- recuperación ante fallos;
- pruebas de restauración.

## Privacidad

La implementación deberá definir políticas de conservación y tratamiento de información de clientes, pedidos, pagos y entregas de acuerdo con las obligaciones legales aplicables.
