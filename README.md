# Normalizacion de tablas 



## Primera Forma Normal 

Identificar las redundancias y datos que no sean atomicos, separar dependencias en tablas mas pequeñas.


**Tabla universidades**

| Id_Universidad | Universidad |
|----------------|-------------|
| 1              | ETITC       |
| 2              | Pedagogica  |
| 3              | Unicolmayor |

**Tabla de roles**

| ID_Rol_Usuario | Rol_Usuario    |
|----------------|----------------|
| 1              | Administrativo |
| 2              | Docente        |
| 3              | Estudiante     |

**Tabla tipo vehiculo**

| ID_TIpoVehiculo | Tipo_Vehiculo |
|-----------------|---------------|
| 1               | Automóvil     |
| 2               | Bicicleta     |
| 3               | Motocicleta   |

**Tabla Usuarios**


| Cedula     | Fecha Ingreso | Nombre    | Apellido   | ID_Rol_Usuario | ID_Universidad | ID_Facultad | ID_ipoVehiculo | Imagen_Persona |
|------------|---------------|-----------|------------|----------------|----------------|-------------|----------------|----------------|
| 1023456789 | 13/09/2024    | Juan      | Pérez      | 3              | 2              | 15          | 1              | www.Imagen.com |
| 2034567890 | 13/09/2024    | María     | Gómez      | 2              | 2              | 19          | 3              | www.Imagen.com |
| 3125678901 | 13/09/2024    | Carlos    | Rodríguez  | 1              | 2              | 1           | 1              | www.Imagen.com |
| 4056789012 | 13/09/2024    | Ana       | López      | 3              | 3              | 8           | 2              | www.Imagen.com |
| 5067890123 | 13/09/2024    | Luis      | Martínez   | 2              | 1              | 15          | 1              | www.Imagen.com |
| 6078901234 | 13/09/2024    | Laura     | Sánchez    | 1              | 1              | 15          | 1              | www.Imagen.com |
| 7089012345 | 13/09/2024    | Pedro     | Díaz       | 3              | 1              | 15          | 3              | www.Imagen.com |
| 8090123456 | 13/09/2024    | Sofía     | Torres     | 2              | 2              | 2           | 1              | www.Imagen.com |
| 9101234567 | 13/09/2024    | Javier    | Ramírez    | 1              | 3              | 10          | 1              | www.Imagen.com |
| 1012345678 | 13/09/2024    | Elena     | Morales    | 3              | 1              | 15          | 2              | www.Imagen.com |
| 1123456789 | 14/09/2024    | Andrés    | Jiménez    | 2              | 1              | 15          | 1              | www.Imagen.com |
| 2234567890 | 14/09/2024    | Valentina | Herrera    | 3              | 1              | 9           | 3              | www.Imagen.com |
| 3345678901 | 14/09/2024    | Diego     | Castro     | 1              | 3              | 4           | 1              | www.Imagen.com |
| 4456789012 | 14/09/2024    | Camila    | Ruiz       | 3              | 1              | 15          | 2              | www.Imagen.com |
| 5567890123 | 14/09/2024    | Felipe    | Ortega     | 2              | 3              | 13          | 1              | www.Imagen.com |
| 6678901234 | 14/09/2024    | Gabriela  | Vargas     | 1              | 3              | 7           | 3              | www.Imagen.com |
| 7789012345 | 14/09/2024    | Nicolás   | Mendoza    | 3              | 2              | 21          | 1              | www.Imagen.com |
| 8890123456 | 14/09/2024    | Mariana   | Romero     | 2              | 1              | 15          | 1              | www.Imagen.com |
| 9901234567 | 14/09/2024    | Samuel    | Salazar    | 1              | 3              | 25          | 1              | www.Imagen.com |
| 1012345670 | 14/09/2024    | Paula     | Paredes    | 3              | 3              | 27          | 2              | www.Imagen.com |
| 1123456781 | 15/09/2024    | Mateo     | Cordero    | 2              | 2              | 26          | 1              | www.Imagen.com |
| 2234567892 | 15/09/2024    | Isabela   | Aguirre    | 3              | 1              | 25          | 3              | www.Imagen.com |
| 3345678903 | 15/09/2024    | Santiago  | Ríos       | 1              | 3              | 6           | 1              | www.Imagen.com |
| 4456789014 | 15/09/2024    | Victoria  | Soto       | 3              | 2              | 3           | 2              | www.Imagen.com |
| 5567890125 | 15/09/2024    | Emiliano  | Peña       | 2              | 1              | 25          | 1              | www.Imagen.com |
| 6678901236 | 15/09/2024    | Renata    | Silva      | 1              | 3              | 24          | 3              | www.Imagen.com |
| 7789012347 | 15/09/2024    | Martín    | León       | 3              | 2              | 20          | 1              | www.Imagen.com |
| 8890123458 | 15/09/2024    | Juliana   | Ceballos   | 2              | 1              | 25          | 1              | www.Imagen.com |
| 9901234569 | 15/09/2024    | Esteban   | Franco     | 1              | 3              | 17          | 1              | www.Imagen.com |
| 1012345671 | 15/09/2024    | Natalia   | Medina     | 3              | 2              | 12          | 2              | www.Imagen.com |
| 1123456782 | 16/09/2024    | Joaquín   | Castillo   | 2              | 1              | 25          | 1              | www.Imagen.com |
| 2234567893 | 16/09/2024    | Valeria   | Jiménez    | 3              | 3              | 16          | 3              | www.Imagen.com |
| 3345678904 | 16/09/2024    | Cristian  | Delgado    | 1              | 2              | 23          | 1              | www.Imagen.com |
| 4456789015 | 16/09/2024    | Mariana   | Aguayo     | 3              | 1              | 25          | 2              | www.Imagen.com |
| 5567890126 | 16/09/2024    | Leonardo  | Villalobos | 2              | 3              | 22          | 1              | www.Imagen.com |
| 6678901237 | 16/09/2024    | Teresa    | Castañeda  | 1              | 2              | 14          | 3              | www.Imagen.com |
| 7789012348 | 16/09/2024    | Hugo      | Quiroz     | 3              | 1              | 25          | 1              | www.Imagen.com |
| 8890123459 | 16/09/2024    | Lucía     | Zamora     | 2              | 3              | 13          | 1              | www.Imagen.com |
| 9901234570 | 16/09/2024    | Felipe    | Arrieta    | 1              | 2              | 4           | 1              | www.Imagen.com |
| 1012345672 | 16/09/2024    | Sofía     | Salinas    | 3              | 1              | 25          | 2              | www.Imagen.com |
| 1123456783 | 17/09/2024    | Gonzalo   | Cortés     | 2              | 3              | 9           | 1              | www.Imagen.com |
| 2234567894 | 17/09/2024    | Alejandra | Becerra    | 3              | 2              | 11          | 3              | www.Imagen.com |
| 3345678905 | 17/09/2024    | Ricardo   | Montoya    | 1              | 1              | 25          | 1              | www.Imagen.com |
| 4456789016 | 17/09/2024    | Sara      | Rojas      | 3              | 3              | 8           | 3              | www.Imagen.com |
| 5567890127 | 17/09/2024    | Iván      | Salgado    | 2              | 2              | 5           | 1              | www.Imagen.com |
| 6678901238 | 17/09/2024    | Clara     | Aguirre    | 1              | 2              | 25          | 3              | www.Imagen.com |
| 7789012349 | 17/09/2024    | Tomás     | Pineda     | 3              | 3              | 21          | 1              | www.Imagen.com |
| 8890123460 | 17/09/2024    | Paula     | Cordero    | 2              | 3              | 18          | 1              | www.Imagen.com |
| 9901234571 | 17/09/2024    | Nicolás   | Salas      | 1              | 1              | 25          | 2              | www.Imagen.com |
| 1012345673 | 18/09/2024    | Mariana   | Castro     | 2              | 1              | 25          | 3              | www.Imagen.com |

**tabla de facultades**

| Id_Universidad | Facultad            |   | Facultad            | Id_Facultad |
|----------------|---------------------|---|---------------------|-------------|
| 2              | Ingeniería          |   | Administración      | 1           |
| 2              | Medicina            |   | Arquitectura        | 2           |
| 2              | Administración      |   | Artes               | 3           |
| 3              | Derecho             |   | Biblioteca          | 4           |
| 1              | Ingeniería          |   | Biología            | 5           |
| 1              | Ingeniería          |   | Contabilidad        | 6           |
| 1              | Ingeniería          |   | Deportes            | 7           |
| 2              | Arquitectura        |   | Derecho             | 8           |
| 2              | Finanzas            |   | Economía            | 9           |
| 1              | Ingeniería          |   | Finanzas            | 10          |
| 1              | Ingeniería          |   | Física              | 11          |
| 1              | Economía            |   | Fisioterapia        | 12          |
| 3              | Biblioteca          |   | Historia            | 13          |
| 1              | Ingeniería          |   | Informática         | 14          |
| 3              | Historia            |   | Ingeniería          | 15          |
| 3              | Deportes            |   | Ingeniería Civil    | 16          |
| 2              | Odontología         |   | Marketing           | 17          |
| 1              | Ingeniería          |   | Matemáticas         | 18          |
| 3              | Sistemas            |   | Medicina            | 19          |
| 3              | Veterinaria         |   | Nutrición           | 20          |
| 2              | Sociología          |   | Odontología         | 21          |
| 1              | Sistemas            |   | Psicología          | 22          |
| 3              | Contabilidad        |   | Recursos Humanos    | 23          |
| 2              | Artes               |   | Relaciones Públicas | 24          |
| 1              | Sistemas            |   | Sistemas            | 25          |
| 3              | Relaciones Públicas |   | Sociología          | 26          |
| 2              | Nutrición           |   | Veterinaria         | 27          |
| 1              | Sistemas            |   
| 3              | Marketing           |   
| 2              | Fisioterapia        |   
| 1              | Sistemas            |   
| 3              | Ingeniería Civil    |   
| 2              | Recursos Humanos    |   
| 1              | Sistemas            |   
| 3              | Psicología          |   
| 2              | Informática         |   
| 1              | Sistemas            |   
| 3              | Historia            |   
| 2              | Biblioteca          |   
| 1              | Sistemas            |   
| 3              | Economía            |   
| 2              | Física              |   
| 1              | Sistemas            |   
| 3              | Derecho             |   
| 2              | Biología            |   
| 2              | Sistemas            |   
| 3              | Odontología         |   
| 2              | Matemáticas         |   
| 1              | Sistemas            |   
| 1              | Sistemas            |   

## Segunda forma normal

Identificar las llaves primarias y dependencias parciales.


**Tabla de informacion_usuarios**

En esta tabla todos los datos dependen de la llave primaria "cedula".

| Cedula     | Nombre    | Apellido   | ID_Tipo_Usuario | ID_Universidad | ID_Facultad | Imagen         | Id_Registro |
|------------|-----------|------------|-----------------|----------------|-------------|----------------|-------------|
| 1023456789 | Juan      | Pérez      | 3               | 2              | 15          | www.Imagen.com | 1           |
| 2034567890 | María     | Gómez      | 2               | 2              | 19          | www.Imagen.com | 2           |
| 3125678901 | Carlos    | Rodríguez  | 1               | 2              | 1           | www.Imagen.com | 3           |
| 4056789012 | Ana       | López      | 3               | 3              | 8           | www.Imagen.com | 4           |
| 5067890123 | Luis      | Martínez   | 2               | 1              | 15          | www.Imagen.com | 5           |
| 6078901234 | Laura     | Sánchez    | 1               | 1              | 15          | www.Imagen.com | 6           |
| 7089012345 | Pedro     | Díaz       | 3               | 1              | 15          | www.Imagen.com | 7           |
| 8090123456 | Sofía     | Torres     | 2               | 2              | 2           | www.Imagen.com | 8           |
| 9101234567 | Javier    | Ramírez    | 1               | 3              | 10          | www.Imagen.com | 9           |
| 1012345678 | Elena     | Morales    | 3               | 1              | 15          | www.Imagen.com | 10          |
| 1123456789 | Andrés    | Jiménez    | 2               | 1              | 15          | www.Imagen.com | 11          |
| 2234567890 | Valentina | Herrera    | 3               | 1              | 9           | www.Imagen.com | 12          |
| 3345678901 | Diego     | Castro     | 1               | 3              | 4           | www.Imagen.com | 13          |
| 4456789012 | Camila    | Ruiz       | 3               | 1              | 15          | www.Imagen.com | 14          |
| 5567890123 | Felipe    | Ortega     | 2               | 3              | 13          | www.Imagen.com | 15          |
| 6678901234 | Gabriela  | Vargas     | 1               | 3              | 7           | www.Imagen.com | 16          |
| 7789012345 | Nicolás   | Mendoza    | 3               | 2              | 21          | www.Imagen.com | 17          |
| 8890123456 | Mariana   | Romero     | 2               | 1              | 15          | www.Imagen.com | 18          |
| 9901234567 | Samuel    | Salazar    | 1               | 3              | 25          | www.Imagen.com | 19          |
| 1012345670 | Paula     | Paredes    | 3               | 3              | 27          | www.Imagen.com | 20          |
| 1123456781 | Mateo     | Cordero    | 2               | 2              | 26          | www.Imagen.com | 21          |
| 2234567892 | Isabela   | Aguirre    | 3               | 1              | 25          | www.Imagen.com | 22          |
| 3345678903 | Santiago  | Ríos       | 1               | 3              | 6           | www.Imagen.com | 23          |
| 4456789014 | Victoria  | Soto       | 3               | 2              | 3           | www.Imagen.com | 24          |
| 5567890125 | Emiliano  | Peña       | 2               | 1              | 25          | www.Imagen.com | 25          |
| 6678901236 | Renata    | Silva      | 1               | 3              | 24          | www.Imagen.com | 26          |
| 7789012347 | Martín    | León       | 3               | 2              | 20          | www.Imagen.com | 27          |
| 8890123458 | Juliana   | Ceballos   | 2               | 1              | 25          | www.Imagen.com | 28          |
| 9901234569 | Esteban   | Franco     | 1               | 3              | 17          | www.Imagen.com | 29          |
| 1012345671 | Natalia   | Medina     | 3               | 2              | 12          | www.Imagen.com | 30          |
| 1123456782 | Joaquín   | Castillo   | 2               | 1              | 25          | www.Imagen.com | 31          |
| 2234567893 | Valeria   | Jiménez    | 3               | 3              | 16          | www.Imagen.com | 32          |
| 3345678904 | Cristian  | Delgado    | 1               | 2              | 23          | www.Imagen.com | 33          |
| 4456789015 | Mariana   | Aguayo     | 3               | 1              | 25          | www.Imagen.com | 34          |
| 5567890126 | Leonardo  | Villalobos | 2               | 3              | 22          | www.Imagen.com | 35          |
| 6678901237 | Teresa    | Castañeda  | 1               | 2              | 14          | www.Imagen.com | 36          |
| 7789012348 | Hugo      | Quiroz     | 3               | 1              | 25          | www.Imagen.com | 37          |
| 8890123459 | Lucía     | Zamora     | 2               | 3              | 13          | www.Imagen.com | 38          |
| 9901234570 | Felipe    | Arrieta    | 1               | 2              | 4           | www.Imagen.com | 39          |
| 1012345672 | Sofía     | Salinas    | 3               | 1              | 25          | www.Imagen.com | 40          |
| 1123456783 | Gonzalo   | Cortés     | 2               | 3              | 9           | www.Imagen.com | 41          |
| 2234567894 | Alejandra | Becerra    | 3               | 2              | 11          | www.Imagen.com | 42          |
| 3345678905 | Ricardo   | Montoya    | 1               | 1              | 25          | www.Imagen.com | 43          |
| 4456789016 | Sara      | Rojas      | 3               | 3              | 8           | www.Imagen.com | 44          |
| 5567890127 | Iván      | Salgado    | 2               | 2              | 5           | www.Imagen.com | 45          |
| 6678901238 | Clara     | Aguirre    | 1               | 2              | 25          | www.Imagen.com | 46          |
| 7789012349 | Tomás     | Pineda     | 3               | 3              | 21          | www.Imagen.com | 47          |
| 8890123460 | Paula     | Cordero    | 2               | 3              | 18          | www.Imagen.com | 48          |
| 9901234571 | Nicolás   | Salas      | 1               | 1              | 25          | www.Imagen.com | 49          |
| 1012345673 | Mariana   | Castro     | 2               | 1              | 25          | www.Imagen.com | 50          |

**Tabla de registro_ingreso_parqueadero**

En esta tabla los datos dependen de la llave primaria "Id_Registro"

| Id_Registro | Id_Cedula  | ID_Vehiculo | Fecha Ingreso |
|-------------|------------|-------------|---------------|
| 1           | 1023456789 | 1           | 13/09/2024    |
| 2           | 2034567890 | 3           | 13/09/2024    |
| 3           | 3125678901 | 1           | 13/09/2024    |
| 4           | 4056789012 | 2           | 13/09/2024    |
| 5           | 5067890123 | 1           | 13/09/2024    |
| 6           | 6078901234 | 1           | 13/09/2024    |
| 7           | 7089012345 | 3           | 13/09/2024    |
| 8           | 8090123456 | 1           | 13/09/2024    |
| 9           | 9101234567 | 1           | 13/09/2024    |
| 10          | 1012345678 | 2           | 13/09/2024    |
| 11          | 1123456789 | 1           | 14/09/2024    |
| 12          | 2234567890 | 3           | 14/09/2024    |
| 13          | 3345678901 | 1           | 14/09/2024    |
| 14          | 4456789012 | 2           | 14/09/2024    |
| 15          | 5567890123 | 1           | 14/09/2024    |
| 16          | 6678901234 | 3           | 14/09/2024    |
| 17          | 7789012345 | 1           | 14/09/2024    |
| 18          | 8890123456 | 1           | 14/09/2024    |
| 19          | 9901234567 | 1           | 14/09/2024    |
| 20          | 1012345670 | 2           | 14/09/2024    |
| 21          | 1123456781 | 1           | 15/09/2024    |
| 22          | 2234567892 | 3           | 15/09/2024    |
| 23          | 3345678903 | 1           | 15/09/2024    |
| 24          | 4456789014 | 2           | 15/09/2024    |
| 25          | 5567890125 | 1           | 15/09/2024    |
| 26          | 6678901236 | 3           | 15/09/2024    |
| 27          | 7789012347 | 1           | 15/09/2024    |
| 28          | 8890123458 | 1           | 15/09/2024    |
| 29          | 9901234569 | 1           | 15/09/2024    |
| 30          | 1012345671 | 2           | 15/09/2024    |
| 31          | 1123456782 | 1           | 16/09/2024    |
| 32          | 2234567893 | 3           | 16/09/2024    |
| 33          | 3345678904 | 1           | 16/09/2024    |
| 34          | 4456789015 | 2           | 16/09/2024    |
| 35          | 5567890126 | 1           | 16/09/2024    |
| 36          | 6678901237 | 3           | 16/09/2024    |
| 37          | 7789012348 | 1           | 16/09/2024    |
| 38          | 8890123459 | 1           | 16/09/2024    |
| 39          | 9901234570 | 1           | 16/09/2024    |
| 40          | 1012345672 | 2           | 16/09/2024    |
| 41          | 1123456783 | 1           | 17/09/2024    |
| 42          | 2234567894 | 3           | 17/09/2024    |
| 43          | 3345678905 | 1           | 17/09/2024    |
| 44          | 4456789016 | 3           | 17/09/2024    |
| 45          | 5567890127 | 1           | 17/09/2024    |
| 46          | 6678901238 | 3           | 17/09/2024    |
| 47          | 7789012349 | 1           | 17/09/2024    |
| 48          | 8890123460 | 1           | 17/09/2024    |
| 49          | 9901234571 | 2           | 17/09/2024    |
| 50          | 1012345673 | 3           | 18/09/2024    |
