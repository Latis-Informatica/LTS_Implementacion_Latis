# Instalar SQL Server 2005

Instalación de SQL Server 2005 para Latis

- Al iniciar la instalación, si aparece el siguiente mensaje hacer click en <kbd>Ejecutar programa</kbd>

![fig 1 SQL Server](../img/SQL_Server_2005/Fig01.png)

- Aceptar los términos u condiciones y hacer click en <kbd>Siguiente</kbd> para continuar.

![fig 2 SQL Server](../img/SQL_Server_2005/Fig02.png)

![fig 4 SQL Server](../img/SQL_Server_2005/Fig04.png)

- Si no hay ningún error hacer click en <kbd>Siguiente</kbd> .

![fig 5 SQL Server](../img/SQL_Server_2005/Fig05.png)

- Hacer click en <kbd>Siguiente</kbd>.

![fig 6 SQL Server](../img/SQL_Server_2005/Fig06.png)

- Presionar <kbd>Siguiente</kbd>.

- Llenar la información de registro.
  
![fig 7 SQL Server](../img/SQL_Server_2005/Fig07.png)

- Presionar <kbd>Siguiente</kbd> para comenzar.


![fig 8 SQL Server](../img/SQL_Server_2005/Fig08.png)
>La instalación recomendada es la indicada a continuación:

- Servicios de bases de datos
- Hacer click en <kbd>Avanzadas</kbd>.

- Seleccionar Archivo de datos.

![fig 9 SQL Server](../img/SQL_Server_2005/Fig09.png)

- Y hacer click en <kbd>Examinar</kbd>

En Windows, crear una carpeta SQLData en el disco duro donde se va a montar la base de datos.
```
Ej: C:\SQLData
```

![fig 10 SQL Server](../img/SQL_Server_2005/Fig10.png)

- Y seleccionar la como Ruta de instalación. Y hacer click en <kbd>Aceptar</kbd>.

![fig 11 SQL Server](../img/SQL_Server_2005/Fig11.png)
- Seleccionar la instancia predeterminada
- Y darle <kbd>Siguiente</kbd>
  
![fig 12 SQL Server](../img/SQL_Server_2005/Fig12.png)

- Seleccionar la cuenta del sistema.
- Y darle <kbd>Siguiente</kbd>.

![fig 13 SQL Server](../img/SQL_Server_2005/Fig13.png)

> **IMPORTANTE**: Para que Latis/Pro funcione correctamente se debe seleccionar el Modo mixto.

- Seleccionar el Modo de autenticación Mixto
- Escribir la contraseña para el usuario **SA** de SQL Server.
- Darle <kbd>Siguiente</kbd>
    
![fig 14 SQL Server](../img/SQL_Server_2005/Fig14.png)

- Se debe seleccionar el "collation" o "intercalación" Latin1_General y "Distingue acentos"
- Darle <kbd>Siguiente</kbd>
  
![fig 15 SQL Server](../img/SQL_Server_2005/Fig15.png)


![fig 17 SQL Server](../img/SQL_Server_2005/Fig17.png)
- Esperar a que termine la instalación

Dependiendo de la versión de Windows puede aparecer el 
siguiente mensaje:
![fig 16a SQL Server](../img/SQL_Server_2005/Fig16a.png)

- Darle click en <kbd>Ejecutar programa</kbd>

Una vez instalados todos los componentes

![fig 19 SQL Server](../img/SQL_Server_2005/Fig19.png)

- Darle click en <kbd>Siguiente</kbd>

![fig 20 SQL Server](../img/SQL_Server_2005/Fig20.png)

- Darle click en <kbd>Finalizar</kbd>

[Volver a Línea base](../Linea_Base.md)