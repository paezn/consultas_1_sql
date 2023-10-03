# consultas_1_sql
# Introducción a las consultas a una BD usando el lenguaje SQL

## Base de datos: Ventas
## Tabla: Cliente

![Tabla Cliente](tabla_Cliente.png "Tabla Cliente")

## Instruccion SELECT
- Permite seleccionar datos de una tabla.
- Su formato es: `SELECT campos_tabla FROM nombre_tabla`

### Consulta No. 1
1. Para visualizar toda la información que contiene la tabla Cliente se puede incluir con la instrucción SELECT el carácter **\*** o cada uno de los campos de la tabla.

- `SELECT * FROM Cliente`
![Consulta1](consulta1_1.png "Consulta 1 - 1")

- `SELECT identificacion, nombre, apellidos, direccion, telefono, ciudad_nac, fecha_nac FROM Cliente`
![Consulta1](consulta1_2.png "Consulta 1 - 2")

### Consulta No. 2

2. Para visualizar solamente la identificacion del Cliente: `SELECT identificacion FROM Cliente`
![Consulta2](consulta2.png "Consulta 2")

### Consulta No. 3

3. Si se desea obtener los registros cuya identificacion sea mayor o igual a 150, se debe utilizar la cláusula `WHERE` que especifica las condiciones que deben reunir los registros que se van a seleccionar: `SELECT * FROM Cliente WHERE identificacion>=150`

![Consulta3](consulta3.png "Consulta 3")

### Consulta No. 4

4. Se desea obtener los registros cuyos apellidos sean Vanegas o Cetina, se debe utilizar el operador `IN` que especifica los registros que se quieren visualizar de una tabla.

`SELECT apellidos, nombre FROM Cliente WHERE apellidos IN('Vanegas', 'Cetina')`

![Consulta4_1](consulta4_1.png "Consulta 4_1")

O se puede utilizar el operador `OR`

`SELECT apellidos, nombre FROM Cliente WHERE apellidos = 'Vanegas' OR apellidos = 'Cetina'`

![Consulta4_2](consulta4_2.png "Consulta 4_2")

### Consulta No. 5

5. Se desea obtener los registros cuya identificación sea menor de 110 y la ciudad sea Cali, se debe utilzar el operador `AND`

`SELECT * FROM Cliente WHERE identificacion<=110 AND ciudad_nac = 'Cali'`

![Consulta5](consulta5.png "Consulta 5")


### Consulta No. 6

6. Si se desea obtener los registros cuyos nombres empiecen por la letra 'A', se debe utilizar el operador `LIKE` que utiliza los patrones `%` (todos) y `_` (caracter).

`SELECT * FROM Cliente WHERE nombre LIKE 'A%'`

![Consulta6](consulta6.png "Consulta 6")


