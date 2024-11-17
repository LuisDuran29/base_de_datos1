# Normalizacion de tablas 

Organizar los datos de una base de datos de manera que cumplan con ciertas reglas o formas normales.

## Primera Forma Normal 

Identificar las redundancias y datos que no sean atomicos, separar dependencias en tablas mas pequeñas.

En esta se tabla se encuentra con datos crudos en la que podemos evidenciar redundancias en algunos campos.

![datos crudos](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/datos_crudos.png)

Agrupamos los datos en diferetes tablas para que nos sea mas facil identificar las dependencias.

![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/organizar_info.png)
![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/organizar_vehiculo.png)
![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/organizar_ingreso.png)

ya agrupados los datos creamos tablas separadas para conjunto de datos relacionados.

**Tabla universidades**

![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/universidad.png)

**Tabla de roles**

![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/rol_usuario.png)

**Tabla tipo vehiculo**

![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/tipo_vehiculo.png)

**Tabla Usuarios**

![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/datos_usuarios.png)

**tabla de facultades**

![datos organizados](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/facultades.png)

## Segunda forma normal

Identificar las llaves primarias y dependencias parciales.


**Tabla de informacion_usuarios**

En esta tabla todos los datos dependen de la llave primaria "cedula".
![dependendias](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/dependencia_2fn.png)

**Tabla de registro_ingreso_parqueadero**

En esta tabla los datos dependen de la llave primaria "Id_Registro"

![dependencias](https://github.com/LuisDuran29/base_de_datos1/blob/main/imagenes/dependencia1_2fn.png)
