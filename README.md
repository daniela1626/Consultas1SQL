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
