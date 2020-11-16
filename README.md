# Ciclo SQL - MisionTic2022

![MisionTic2022](MisionTic2022.png)

[Ir al sitio web del programa Mision Tic 2022](https://www.misiontic2022.gov.co/portal/)

Consultas SQL a Base de Datos relacional y su implementación en lenguaje JAVA a través del Java DataBase Connectivity - JDBC.

## Orden secuencial de las Sentencias de una consulta:
1. SELECT
2. FROM
3. JOINT ON
4. WHERE
5. GROUPBY
6. HAVING
7. ORDER BY

- Operadores Logicos: 
{ =,<>,>,<,<=,>=, And, Or, Like, Between, In}

- Data Manipulation Language (DML): 
{ SELECT, UPDATE, DELETE}

- Data Definition Language (DDL): 
{ (CREATE|ALTER|TRUNCATE)DATABASE, (CREATE|ALTER|DROP)TABLE, (CREATE|DROP)INDEX }

- Funciones de agrupamiento:
COUNT: Contar datos, MAX: El máximo de los datos, MIN: El mínimo de los datos, AVG: El promedio de los datos, SUM: La suma de los datos, VAR: La varianza de los datos, STDEV: La desviación estándar de los datos.

- Funciones de no agrupamiento:
UCase( ) or UPPER(), LCase( ), Mid( ), Len( ) OR LENGTH (), Round( ), Concatenar, First( ), Last( ), Now( ), Format( ), Substr(), InStr( ), InStrRev( ), Left( ), Right( ).

## JDBC: Uso básico

1. Crear una conexión a la base de datos:
Archivo de configuración para la conexión especificando, localización física de la base de datos, controlador (driver), conexión Objeto de clase Connection (JDBC). 

2. Crear una instrucción SQL:
Objeto de la clase Statement (JDBC) recurre al método .createStatement() de la clase Connection (JDBC).

3. Utilizar la conexión para enviar por ahí las instrucciones en SQL:
Objeto de la clase ResultSet recurre al método .execute() para crear tablas, or .executeQuery() para ejercutar consultas, or .executeUpdate() para actulizar datos y finalmente close( ) para cerrar la instruccion.

Con el método next( ) se avanza sobre la secuencia resultante, con los métodos getString( ) y getInt( ) se extrae la información de los campos del elemento actual de la secuencia. 

Se usa if (resultado.next( )) para acceder al elemento retornado por la sentencia SQL. Se usa ademas while (resultado.next( )) para acceder a los elementos retornados por la sentencia SQL. 