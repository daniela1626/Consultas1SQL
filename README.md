# consultas1.SQL

# EJERCICIOS CONSULTAS SQL

## Tabla de usuario

![Usuario](img/captura.jpeg "Usuario")

1. Para visualizar toda la informacion que contiene la tabla `usuario` se puede incluir con la instruccion SELECT el caracter'*' o cada uno de los campos 

SELECT * FROM `Usuario` 

![Consulta1](img/1.jpeg "Consulta1")

2. Visualizar solamente la identificacion del usuario 

SELECT `identificacion` FROM `Usuario` 

![Consulta2](img/2.jpeg "Consulta2")

3. Se desea obtener los registros cuya identificacion sean mayorres o iguales a 150, se debe utilizar la clausula WHere que especifica las condiciones que debe reunir los registros que se van a seleccionar 

SELECT * FROM `Usuario` WHERE identificacion>=`150`

![Consulta3](img/3.jpeg "Consulta3")

4. Si se desea obtener los rgistros cuyo sus apellidos sean Vanegas o Cetina, se debe utilizar el operador IN que especifica los registros que se quieren visualizar en la tabla

`select apellidos from Usuario where apellidos IN('Vanegas', 'Cetina')`

![Consulta 4](img/4.jpeg "Consulta 4")

O se puede utilizar el operador OR

`select apellido from Usuario where apellido='Vanegas' or apellido='Cetina'`

![Consulta 4](img/4_1.jpeg "Consulta 4")

5. SI se desea obtener los registros cuya identificacion sea menor de `110` y la ciudad sea CAli se debe utilizar el operador AND.

`SELECT * FROM usuario  WHERE Identificacion<`150` AND ciudad=`Cali`

![Consulta 5](img/5.png "Consulta 5")


6. Si se desa obtener los registros cuyos nombres empiecen por la letra a, sebe utilizar l operador LIKE que utiliza los patrones "%" (todos) y '_' (caracter)

`select * from Usuario where nombre LIKE 'A%'`

![Consulta 6](img/6.jpeg "Consulta 6")

7. Se desea obtener los registros cuyos nombres tengan la letra a 

`select * from Usuario where nombre LIKE '%a%'`

![Consulta 7](img/7.jpeg "Consulta 7")


8. Si se desea obtener los regisro donde la cuarta letra de nomre sea una a

`select * from Usuario where nombre LIKE '___a%'`

![Consulta 8](img/8.jpeg "Consulta 8")

9. Si se desea obtener los registros cuya identificaci??n este entre el intervalo 110 y 150, se debe utilizar la clausula BETWEEN, que sirve para especificr un intervalo de valores

`select * from Usuario where identificacion BETWEEN '110' and '150'`

![Consulta 9](img/9.jpeg "Consulta 9")

## COMANDO DELETE

10. Para eleminar solamente los registros cuya identificaci??n sea mayor de 130 

`delete from Usuario where identficacion>'130'`

![Consulta 10](img/10.jpeg "Consulta 10")

![Consulta 10](img/10_1.jpeg "Consulta 10")

## COMANDO UPDATE

11. Para actualizar la ciudad de nacimiento de Cristian Vanegas cuya identificaci??n es 114

`update Usuario set ciudad_nac = 'Manisalez' where identificacion='114'`

![Consulta 11](img/11.jpeg "Consulta 11")

![Consulta 11](img/11_1.jpeg "Consulta 11")