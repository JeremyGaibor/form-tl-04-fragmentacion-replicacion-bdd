# Práctica de fragmentación de base de datos distribuida

## Descripción

Esta práctica implementa una base de datos distribuida para una cafetería universitaria mediante PostgreSQL 16 y Docker Compose.

Se utilizan tres nodos independientes:

- `pg-campus`: sede Campus.
- `pg-babahoyo`: sede Babahoyo.
- `pg-ventanas`: sede Ventanas.

La práctica incluye:

- Esquema centralizado.
- Fragmentación horizontal de la tabla `pedidos`.
- Fragmentación vertical de la tabla `clientes`.
- Fragmentación mixta.
- Reconstrucción global mediante `postgres_fdw`.
- Verificación de completitud, reconstrucción y disjunción.

---

## Tecnologías utilizadas

- Docker Desktop.
- Docker Compose.
- PostgreSQL 16 Alpine.
- DBeaver.
- CMD de Windows.
- IntelliJ IDEA.
- Git y GitHub.

---

## Estructura del proyecto

```text
practica-fragmentacion/
├── docker-compose.yml
└── sql/
    ├── 01_esquema_central.sql
    ├── 02_datos.sql
    ├── 03_fragmentacion_horizontal.sql
    ├── 04_fragmentacion_vertical.sql
    ├── 05_fragmentacion_mixta.sql
    ├── 06_vistas_globales.sql
    └── 07_verificacion.sql
