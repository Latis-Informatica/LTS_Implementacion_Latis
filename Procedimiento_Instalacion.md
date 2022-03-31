# **PROCEDIMIENTO** DE INSTALACION LATIS/PRO MARZO DEL 2022

## Certificación de la factibilidad de instalación

- [ ] Descargar documentos de soporte desde la pagina Web del sistema **[LatisPro](https://www.latisinformatica.com/Integradores/Descargas)**
  - [ ] Lista de verificación para instalación del sistema  Latis/Pro
  - [ ] Procedimiento de verificación para elementos de la lista de verificación
  - [ ] Procedimiento de instalación sistema Latis/Pro
- [ ] Certificar que todos y cada uno de los elementos de la lista han sido satisfechos. En caso contrario se debe informar al responsable de la implementación cual elemento de la lista ha fallado y en base a lo establecido en el [procedimiento de verificación](https://www.latisinformatica.com/Integradores/Descargas) corregir para proseguir con la instalación.  



## Descarga de componentes necesario para la instalación

- [ ] Una vez certificado el cumplimiento de todos los elementos de la lista de verificación se deben seguir los siguientes pasos:
  - [ ] Crear una carpeta LatisPro_Instaladores 

  - [ ] Realizar las siguientes descargas desde la pagina de [LatisPro](https://www.latisinformatica.com/Integradores/Descargas) y copiar en la carpeta LatisPro_Instaladores
    - [ ] [Instalador de Latis](https://www.latisinformatica.com/Integradores/Descargas/App/Instalador Lattice 1.8.rar) -  Instalador de Mayo 2010
    - [ ] Si el sql server es 2008 o superior se debe descargar 
      - [ ] [Tool - Configuración de Servidor](https://www.latisinformatica.com/Integradores/Descargas/Apps/setupCfgSrv2018.zip) -  Nueva versión de configuración de Servidor Latis para SQL Server 2008 o superior
    - [ ] [Actualizador 2021](https://www.latisinformatica.com/Integradores/Descargas/Apps/ActObtHttp.zip) - Ultima versión del programa Actualizador para manejar problemas con https y DM Aplicar (DMApl.exe).
    - [ ] [Configuración de servidor](https://www.latisinformatica.com/Fixs/tools/CfgSrv.zip) - Ultima versión de configuración de servidor de Latis/Pro versiones de sql inferior al 2008.
    - [ ] [Tool - Configuración de Servidor](https://www.latisinformatica.com/Integradores/Descargas/Apps/setupCfgSrv2018.zip) -  Nueva versión de configuración de Servidor Latis para SQL Server 2008 o superior
    - [ ] [ Tool - SQLBak Lite](https://www.latisinformatica.com/Integradores/Descargas/Apps/setupSQLBakLite.zip) -  Programa para respaldo de base de datos Latis. Incluye programación automática en 'Tareas Programadas' de Windows
    - [ ] [ Tool - SQLRestore Lite](https://www.latisinformatica.com/Integradores/Descargas/Apps/setupSQLRestoreLite.rar) - Programa para restauración de bases de datos de SQL Server.
    - [ ] SI el servidor puede ser usado como equipo de trabajo para emisión de reportes o consultas se debe descargar
      - [ ] [DLL de List & Label](https://www.latisinformatica.com/Integradores/Descargas/Apps/LL.zip) -  DLL para exportación de documentos para List & Label
      - [ ] [DLL de vbZip y vbUnzip](https://www.latisinformatica.com/Integradores/Descargas/Apps/vbzip.zip) - Para uso en la Consulta Directa de Latis. (En caso de error: "Tip - Dif", copiar estos archivos en la carpeta de instalación de Latis)
    
    Es necesario descargar e instalar las siguientes aplicaciones de terceros:
    
    - [ ] [ WinRAR](https://www.latisinformatica.com/Integradores/Descargas/Apps/wrar401.zip) - Programa para comprimir y descomprimir archivos .RAR
    
    - [ ] [ AnyDesk](https://www.latisinformatica.com/Integradores/Descargas/Apps/AnyDesk.zip) -  Any Desk soporte **remoto**
    
      

## **Instalación del servidor Latis** 

Se debe instalar la aplicación **Winrar** y descomprimir el instalador del sistema dentro de la carpeta LatisPro_Instaladores creada anteriormente.

Se debe Instalar el software **AnyDesk** para recibir soporte remoto durante la instalación.

### Instalación de componentes

Descomprimir el instalador en la carpeta **LatisPro_Instaladores** y descomprimir el instalador. Luego ir a a la carpeta  [Server ](https://www.latisinformatica.com/integradores/Curso/InstLat_InstLatSvc.html) :

- [ ] Ejecutar el setUp.exe y presionar el botón  **[Siguiente]**
- [ ] Suministrar la Información de Usuario y la Organización. Presionar el botón  **[Siguiente]** 
- [ ] Seleccionar tipo de instalación como  [Tipica], Presionar el botón  **[Siguiente]**
- [ ] Al aparecer la pantalla de **"Configuración del servidor Lattice"** se debe presionar el botón **[Salir].** 
- [ ] Una vez culminada la instalación se debe presionar el botón  **[Finalizar]** 
- [ ] Se recomienda ir al botón de la aplicación Latis y en sus propiedades de compatibilidad colocar **"Ejecutar como administrador".**

### Instalación del actualizador de componentes

Descomprimir  ActObtHttp.rar en una carpeta con el mismo nombre dentro de la  carpeta **LatisPro_Instaladores** . Luego se deben copiar todos los archivos que se encuentran en la carpeta ActObtHttp en la carpeta latisPro_Server es decir C:\Program Files (x86)\Latisoft\Lattice Pro Server y reemplazar aquellos archivos existentes.

Luego se debe realizar la siguiente [configuración](https://www.latisinformatica.com/integradores/Curso/InstLat_ActLat.html):

- [ ] Ejecutar el modulo **ActObt.exe** como Administrador

  - [ ] Ir a la pestaña de **[Configuración]**
    - [ ] Seleccionar **Http** como tipo de fuente de datos
    - [ ] Asignar en **Servidor/Directorio Fuente** el directorio donde se encuentran los fixs en el servidor fuente. Por ejemplo: www.latispro.com/Fixs
    - [ ] Asignar **Directorio de trabajo** el directorio  que nos lleva donde esta instalado el sistema.                  Por Ejemplo: C:\Program Files (x86)\Latisoft\Lattice Pro Server\ 
    - [ ] Asignar **Directorio de Fixs** el directorio donde estan instalados los Fixs del sistema.                               Por Ejemplo: C:\Program Files (x86)\Latisoft\Lattice Pro Server\ Fix\
    - [ ] Asignar **Directorio de Winrar** el directorio   donde esta instalado la aplicación winrar.                          Por Ejemplo: C:\Program Files\WinRAR\
    - [ ] Asignar **Prefijo** de la version actual del sistema. Por ejemplo: **"KT4"**
    - [ ] Tildar "Aplicar Fixes" siempre y cuando se desee actualizar el servidor de inmediato. De lo contrario se podría descargar los componentes y luego Aplicar los Fixes.
  - [ ] Ir a la pestaña **"Respaldar Fixs"** y dar clic
  - [ ] Ir a la pestaña **"Descargar**" y dar clic. Verificar que todos los componentes fueron descargados correctamente. Este proceso puede durar algunos minutos dependiendo de la vellosidad de intenet que se disponga al momento de la descarga.
  - [ ] Ir a la pestaña **"Aplicar"** al aparecer el modulo "**Aplicar componentes"** de Latis V-1.?.? se debe precionar el botón **[Aplicar todo]**. Este proceso debe terminar satisfactoria mente y anunciar que esta listo. Si falla se debe realizar alguna de las siguientes acciones:
    - [ ] Verificar que El servicio de procesos programados esta apagado
    - [ ] Verificar que nadie este usando el sistema en este momento y el componente esta apagado.
    - [ ] Si el problema persiste solicite soport experto Nivel II

  

### Instalación del  configurador del servidor y registro de clave

#### Creación de usuario LatisADM

Antes de iniciar la instalación del sistema se debe crear un usuario administrador para Registrar los componentes del sistema

- [ ] Crear usuario administrador LatisADM
- [ ] Incluir en grupo:
  - [ ] Usuarios COM distribuidos
  - [ ] Usuarios Administrador
- [ ] Configurar la contraseña para que no pueda ser modificada y no caduque 



#### Selección del configurador del servidor Latis

 Si la version de Sql Server es 2008 o superior, se debe realizar las siguientes actividades:

- [ ] Ir a la carpeta LatisPro_Instaladores y realizar la extracción de  setupCfgSrv2018.rar a una carpeta del mismo nombre.
- [ ] Ejecutar como administrador el setupCfgSrv2018.exe
- [ ] Ir a la carpeta C:\Program Files (x86)\Latis Informatica\CfgSrv y eje cutar como administrador el CfgSrv.exe

Si la versión del sql server es inferior a 2008 se debe realizar las siguientes tareas:

- [ ]  Extraer del archivo CfgSrv.Zip el archivo CfgSrv.exe y copiarlo a la carpeta C:\Program Files (x86)\Latisoft\Lattice Pro Server sustituyendo el existente.
- [ ] Ejecutar como administrador el archivo para configurar el servidor

Una vez seleccionado el CfgSvr.exe se debe ejecutar como administrador y seguir los siguientes pasos::

- [ ] Ir a la pestaña 5.- Registro de componente 
  - [ ] Registrar los datos del usuario latis y su contraseña
  - [ ] Presionar el botón de **[Procesar]**
- [ ] Ir a la pestaña **1.- Usuario administrador**
  - [ ] Registrar los datos del usuario administrador código, contraseña y descripción
  - [ ] Presionar el botón de **[Procesar]**
- [ ] Ir a la pestaña **2.- Valores iniciales del sistema**
  - [ ] Registrar los datos solicitados;
    - [ ] Código de cliente, proveedor o producto  numérico
    - [ ] Pais de localización 
    - [ ] Longitud del Código de cliente, Documento, Plu,, Producto, Proveedor
    - [ ] Código de moneda de referencia, Moneda del sistema, y tipo de tasa cliente y proveedor 
  - [ ] Presionar el botón de **[Procesar]**
- [ ] Ir a la pestaña **3.- Compañía y sucursal**
  - [ ] Registrar los datos solicitados;
    - [ ] Código de compañia, nombre y razon social.
    - [ ] Código de sucursal y nombre
  - [ ] Presionar el botón de **[Procesar]**
- [ ] Ir a la pestaña **4.- Base de datos**
  - [ ] Registrar los datos solicitados;
    - [ ] Nombre del servidor de base de datos. Se recomienda colocar la palabra (local) como nombre del servidor y (local)\exress
    - [ ] Código del usuario de la base de datos
    - [ ] Contraseña
    - [ ] Nombre de la base de datos
    - [ ] Presionar el botón de **[Conectar]**
    - [ ] SI la base de datos existe selecciones **"Mantener base actual"**
    - [ ] Si la base de datos no existe se debe:
      - [ ] Seleccionar **"Crear base nueva"**
      - [ ] Presionar botón **[Procesar]**
      - [ ] Presionar el botón **[Crear base de soporte]**
  - [ ] Presionar el botón de **[Procesar]**
- [ ] Ir a la pestaña **5.- Registro de componente (Nuevamente)**
  - [ ] Usuario: LatsADM
  - [ ] Contraseña: la creada
  - [ ] Presionar el botón de **[Procesar]**

- [ ] Ir a pestaña de **6.- Monitor de proceso**
  - [ ] Usuario del monitor de proceso: ADM
  - [ ] Contraseña: La colocada al crear usuario Latis
  - [ ] Compañía:  Código de compañía **"01"**
  - [ ] Sucursal: Código de sucursal **"CC"**
  - [ ] Puerto UDP: **1003** (Recomendado)
  - [ ] Presionar el botón de **[Procesar]**

- [ ] Ir a pestaña de **7.- Monitor de Notificación**
  - [ ] Servidor del Monitor: Se recomienda usar dirección IP del servidor (local)
  - [ ] Puerto UDP: 1004 (Recomendado)
  - [ ] Presionar el botón de **[Procesar]**

#### Registro de licencia LatisPro

- [ ] Ir a pestaña de 8.- Registro de licencia
  - [ ] Tarjeta del Servidor : Se recomienda seleccionar la tarjeta de red por la cual esta conectado el servidor o su dirección IP.
  - [ ] Generar archivo de registro:
    - [ ] Se debe presionar el botón de **[Generar archivo para registro],** esto desplegara el administrador de archivo para colocar el nombre y lugar donde quedara el archivo .Dat que contiene la información necesaria para la generación de la Clave de acceso al sistema
    - [ ] Este archivo generado debe ser enviado al departamento de soporte de latis  vía correo electrónico con la siguiente información:
      - [ ] Enviar a : Contacto@LatisInformatica.com
      - [ ] CC: Richard_Reyes@Latisinformatica.com, Gustavo_Galimberti@Latisinformatica.com
      - [ ] Asunto: Registro Empresa "ABC"
      - [ ] Adjuntos: Documento PDF del registro de información fiscal.
      - [ ] Contenido: 
        - [ ] Nro. de Registro de información fiscal 
        - [ ] Razon social
        - [ ] Dirección de la empresa
        - [ ] Telefono de la empresa
        - [ ] Persona Contacto
        - [ ] Telefono Persona contacto
        - [ ] Correo electronico Persona contacto
  - [ ] Registrar Clave:
    - [ ] Se resivira un correo electronico de parte de Latis con el siguiente asunto  **"Regisro empresa ABC** **"**el cual traera en forma anexa la llave de registro se debe:
      - [ ] Descargar el archivo anexo en (.key) en la carpeta Instalador_Latis
      - [ ]  Se debe presionar el botón de **[Registrar Clave]**, esto desplegara el administrador de archivo y permitira buscar y seleccionar el archivo .Key enviado y permitir el acceso al sistema
    - [ ] Si en un Lapso de tiempo no mayor a 72 horas, no has recibido un correo con el archivo de registro y el asunto **"Registro Empresa 'ABC'**" se recomienda:
      - [ ] Llamar al tlf 0212-2390101
      - [ ] Enviar un correo a contacto@latisinformatica.com
      - [ ] Revisar buson de correos "no deseados"



## Instalación del Cliente Latis

Para instalar latisPro en un cliente se debe seguir los siguientes [pasos](https://www.latisinformatica.com/integradores/Curso/InstLat_InstLatClt.html):

- [ ] Verificar accesibilidad al servidor
  - [ ] Se debe presionar las teclas WIN+R
  - [ ] Colocar \\\Nombre servidor\ , 
  - [ ] Presionar  el botón "Aceptar"
  - [ ] Si no se despliega  la carpeta Lattice_Client, debes verificar:
    - [ ] Las [preguntas frecuentes](https://www.latisinformatica.com/Integradores/Faqs)

### Instalación Cliente

En la carpeta Lattice_client se encuentra el istalador se debn seguir los siguientes pasos:

- [ ] Seleccionar la carpeta Lattice_Client
- [ ] Ejecutar como administrador la aplicación Setup.exe
  - [ ] Presionar  el botón "Siguiente"
  - [ ] Ingresar Nombre del usuario 
  - [ ] Ingresar el nombre de la Organización
  - [ ] Presionar  el botón "Siguiente"
  - [ ]  Verifique la carpeta de instalación
  - [ ] Presionar  el botón "Siguiente"
  - [ ] Ingrese el Nombre del servidor o su dirección IP
  - [ ] Presionar  el botón "Siguiente"
  - [ ] Espere unos minutos y luego presionar  el botón "Finalizar"

### Actualización de componentes en el cliente

El instalador del sistema crea un icono de acceso a la aplicación en el escritorio. Se recomienda ir al botón de la aplicación Latis y en sus propiedades de compatibilidad colocar "Ejecutar como administrador".

Al ejecutar el sistema por pimera vez en el Cliente, como administrador, el sistema verifica  contra el servidor y detecta la necesidad de actualizar el cliente se debe autorizar la actualización presionando el boton **[Si]** 



## Instalación de mantenimiento del sistema

Una vez culminada la instalación del servidor y de los clientes se recomienda la instalación del software de mantenimiento de respaldo y restauración de la base de datos con frecuencia de ejecución diaria. También la copia de estos respaldo a unidad de almacenamiento externa para ser llevados fuera de la empresa

### 	Respaldo del sistema

Se deben realizar las siguientes tareas:

- [ ] Instalar SQL BAK LITE:
  - [ ] Ir a la carpeta LatisPro_Instaladores y extraer del  setupSQLBakLite.Zip el archivo setupSQLBakLite.exe y ejecutar como administrador
    - [ ] Verificar la carpeta de instalacon
    - [ ] Presionar el botón **[ Install]** 
    - [ ] Esperar a que culmine la instalación
    - [ ] Presionar botón **[Close]**
    
  - [ ] Ejecute la aplicación SQLBakLite.exe desde  la carpeta C:\Program Files (x86)\Latis Informatica\SQLBakLite  las tareas que permite realizar esta aplicación son:
  
    - [ ] Prueba la conexion con la base de datos.
      - [ ] Al presionar el botón de {conectar] se debe cargar la siguiente información:
        - [ ] Servidor
        - [ ] Usuario de base de datos
        - [ ] Contraseña
        - [ ] Se debe presionar el boton de **[Probar]** para verificar la conexion
      
    - [ ] Parametriza la ejecución del respaldo
    
      | Parametros                                            | Descripción                                                  |
      | ----------------------------------------------------- | ------------------------------------------------------------ |
      | **Archivo de respaldo:**                              | Nombre del archivo de respaldo *Ej: C:\SQLBak\GE_CLT_CCS01.bak`* |
      | **Incluir bases** **adicionales model, master, msdb** | Si está chequeado se incluiran las bases de datos de SQL server model, master, msdb |
      | **Otras bases de datos**                              | Escriba una lista separadas por comas de las bases de datos adiconales que se respaldaran. |
      | **Comprimir archivo de respaldo**                     | Si está chequeado comprime el archivo .bak generado por el respaldo. |
      | **Formato de compresión**                             | SQL: SQL Server (desde SQL Server 2008 o superior)                                                                        RAR:   comprime usando el formato rar. Esto requiere configurar los parámetros ([Ver configuración de WinRAR](https://www.latisinformatica.com/integradores/Curso/Inst_SQLBakLite.html#winrar))                                                                                                                                                       Zip: comprime usando el formato zip |
      | **Borrar archivo de respaldo**                        | Borra el archivo .bak luego de crear el archivo comprimido.  |
      | **Copiar A**                                          | Carpeta donde se copiará el archivo .bak (si no se comprime) o el archivo comprimido (si se comprime). |
      | **Anexar fecha al nombre**                            | Anexar fecha al nombre Si está chequeado le anexa a el nombre de el archivo la fecha del respaldo. |
      | **Borrar respaldos anteriores a**                     | Si está chequeado borrar los archivos respaldados anteriores a los dias indicados. |
      | **Notificar.**                                        | Si está chequeado permite enviar un correo electrónico informando el resultado de la operación de respaldo. Se usa la lista de correos separados por comas indicada en "A:" |
      |                                                       |                                                              |
    

- [ ] Guarda los parametros de emision del respaldo
- [ ] Agrega el SQLBakLite como tarea programada de Windos y configura sus parámetros.
  - [ ] Al presionar este boton se despliega un dialogo donde se debe ingresar la siguiente información
    - [ ] Inicia: Hora de inicio de la tarea
    - [ ] Usuario del sitema: Usuario administrador que ejecuta la tarea.Ejemplo: LatisADM
    - [ ] Contraseña: Contraseña del usuario
    - [ ] Presione el botón **[Ok]**

### 	Restauración del sistema	

Instalar SQL RESTORE LITE:

- [ ] Ir a la carpeta LatisPro_Instaladores y extraer del  setupSQLRestoreLite.Zip el archivo SQLRestoreLite.exe y ejecutar como administrador

  - [ ] Verificar la carpeta de instalacon
  - [ ] Presionar el boton **[ Install]** 
  - [ ] Esperar a que culmine la instalación
  - [ ] Presionar botón **[Close]**

- [ ] Ejecute la aplicación SQLBakLite.exe desde  la carpeta C:\Program Files (x86)\Latis Informatica\SQLRestoreLite  las tareas que permite realizar esta aplicación son:

  - [ ] Prueba la conexión con la base de datos.

    - [ ] Al presionar el botón de {conectar] se debe cargar la siguiente información:
      - [ ] Servidor
      - [ ] Usuario de base de datos
      - [ ] Contraseña
      - [ ] Se debe presionar el boton de **[Probar]** para verificar la conexion

  - [ ] Parametriza la ejecución de la restauración de la base de datos

    | Parametros                         | Descripción                                                  |
    | ---------------------------------- | ------------------------------------------------------------ |
    | **Base de datos**                  | Nombre de la base de datos a ser restaurada                  |
    | **Archivo**                        | Nombre del archivo de respaldo a restaurar debe ser cargado a travez del administrador de archivos. |
    | **Descomprimir en**                | Carpeta en la cual se relizara la descompresion del respaldo |
    | **Registro clave Latis - Archivo** | Carpeta y nombre del archivo que contiene el archivo de regstro Latis |

- [ ] Presionar el botón **[Restaurar]** este proceso pude durar algunos minutos y dependera del tamaño del archivo a restaurar. En la parte inferior del dialogo se presenta el avance de ejecución

- [ ] Una vez restaurada exitosamente la base de datos es necesario que se actualice el la clave de registro. Presione el botón **.[Registrar Key]**

