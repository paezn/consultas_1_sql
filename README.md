# consultas_1_sql
# Introducción a las consultas a una BD usando el lenguaje SQL

## Base de datos: Ventas
## Tabla: Cliente

![Tabla Cliente](tabla_Cliente.png "Tabla Cliente")

## Instruccion SELECT
- Permite seleccionar datos de una tabla.
- Su formato es: `SELECT campos_tabla FROM nombre_tabla``

### Consulta No. 1
1. Para visualizar toda la información que contiene la tabla Cliente se puede incluir con la instrucción SELECT el carácter **\*** o cada uno de los campos de la tabla.

- `SELECT * FROM Cliente`
![Consulta1](consulta1_1.png "Consulta 1 - 1")

- `SELECT identificacion, nombre, apellidos, direccion, telefono, ciudad_nac, fecha_nac FROM Cliente`
![Consulta2](consulta1_2.png "Consulta 1 - 2")


