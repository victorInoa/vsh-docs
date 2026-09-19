# 12 — Arquitectura Multi-Tenant

## Concepto

VSH será una plataforma multi-tenant.

Una instalación de la plataforma administrará múltiples tiendas aisladas lógicamente.

```text
VSH
├── Owner A
│   ├── Store A1
│   └── Store A2
├── Owner B
│   └── Store B1
└── Owner C
    ├── Store C1
    ├── Store C2
    └── Store C3
```

## Aislamiento

Cada tienda debe tener aislamiento de:

- productos;
- inventario;
- sucursales;
- usuarios;
- pedidos;
- configuración;
- reportes.

## Identificación del tenant

Cada request debe resolverse hacia la tienda correspondiente mediante el dominio/subdominio.

Ejemplo:

`zapateria.vsh.do` → Store ZAPATERIA

Con dominio propio:

`www.zapateria.com` → Store ZAPATERIA

## Owner multi-tienda

El Owner tiene una cuenta única y acceso a sus tiendas autorizadas.

Esto evita duplicar cuentas administrativas.

## Seguridad

El aislamiento debe aplicarse también a nivel de autorización y consultas de datos, no solamente en la interfaz.

## Evolución

La arquitectura debe permitir que VSH crezca de decenas a miles de tiendas sin convertir cada nueva tienda en un proyecto independiente.