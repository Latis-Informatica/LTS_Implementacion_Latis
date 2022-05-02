# Instalar SQL Server 2014 Express

Para la instalación de SQL Server 2014 Express:

- Descargar el archivo de instalación adecuado según el idioma del sistema operativo y la arquitectura.

  - Si Windows está en español descargar la de español.
  - Si Windows es de 32Bits descargar x86 si es de 64bits usar el x64.

```
Ej: SQLEXPR_x86_ENU.exe
```
Es para la versión de 32 bits en Ingles.

- Seleccionar "Nueva instalación"
  ![Figura 01](../img/SQL_Server_Express_2014/Fig01.png)


  ![Figura 02](../img/SQL_Server_Express_2014/Fig02.png)

- Aceptar la licencia y darle <kbd>Siguiente</kbd>

  ![Figura 03](../img/SQL_Server_Express_2014/Fig03.png)

- Darle <kbd>Siguiente</kbd>

- En Windows, crear una carpeta **SQLData** en el disco duro donde se va a montar la base de datos.

```
Ej: C:\SQLData
```

  ![Figura 03a](../img/SQL_Server_Express_2014/Fig03a.png)

  ![Figura 04](../img/SQL_Server_Express_2014/Fig04.png)

- Cambiar el Instance root Directory a SQLData

  ![Figura 05](../img/SQL_Server_Express_2014/Fig05.png)

- <kbd>Siguiente</kbd> en el nombre de la instacia de SQL Server.

  ![Figura 06](../img/SQL_Server_Express_2014/Fig06.png)

- Seleccionar **SQL_Latin1_General_CP1_CI_AS** en el Collation.

  ![Figura 07](../img/SQL_Server_Express_2014/Fig07.png)

> **IMPORTANTE**: se debe seleccionar **Modo mixto** y establecer una contraseña, para que la configuración de Latis sea correcta.


- Darle <kbd>Siguiente</kbd>

  ![Figura 08](../img/SQL_Server_Express_2014/Fig08.png)

- Darle <kbd>Close</kbd> para finalizar.

[Volver a Línea base](../Linea_Base.md)