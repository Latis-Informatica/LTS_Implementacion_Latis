# Instalar SQL Server 2008 R2

![fig 1 SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig01.png)
- Seleccionar nueva <kbd>Instalación</kbd> ó <kbd>Installation</kbd>.

  ![fig 1a SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig01a.png)

- Después de las pruebas darle <kbd>Ok</kbd> para continuar.

  ![fig 01b SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig01b.png)
- Luego de introducir el Product key hacer click en <kbd>Install</kbd>
- Si no hay ningún error hacer click en <kbd>Siguiente</kbd>.

  ![fig 02 SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig02.png)
- Seleccionar características de SQL y presionar <kbd>Siguiente</kbd>.
  
- Seleccionar Base de datos y Herramientas de cliente. Como se muestra a continuación.
  
  ![fig 03 SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig03.png)

- Y darle <kbd>Siguiente</kbd>.

- En Windows, crear una carpeta **SQLData** en el disco duro donde se va a montar la base de datos.
  ```
  Ej: C:\SQLData
  ```
  ![fig 03b SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig03b.png)



- En la pantalla de configuración de la Instancia cambiar la ruta a la carpeta **SQLData** y dejar la instancia por defecto.
  
  ![fig 04 SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig04.png)

- Y darle <kbd>Siguiente</kbd>
  
- En la Configuración de Servidor, seleccionar las cuentas de los servicios de SQL.

  ![fig 05 SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig05.png)

- En el collation seleccionar **SQL_Latin1_General_CP1_CI_AS**
  
  ![fig 06 SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig06.png)

Darle <kbd>Siguiente</kdb>.

- En la Configuración de Database Engine Seleccionar **Modo mixto** de autenticación y establecer la contraseña del usuario SA. Adicionalmente agregar el usuario actual como administrador.
  
   ![fig 07 SQL Server 2008 R2](../img/SQL_Server_2008R2/SQL_Fig07.png)

   > **IMPORTANTE**: Para que Latis/Pro funcione correctamente se debe seleccionar el Modo mixto.

- Darle <kbd>Siguiente</kbd>, <kbd>Siguiente</kbd> y luego <kbd>Instalar</kbd>.

[Volver a Línea base](../Linea_Base.md)