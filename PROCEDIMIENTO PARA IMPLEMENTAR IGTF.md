# PROCEDIMIENTO PARA IMPLEMENTAR

#          IMPUESTO A LAS GRANDES 

#      TRANSACCIONES FINANCIERAS

#                (IGTF) ABRIL 2022



- [ ] ## Definir y configurar Impuesto (IGTF)

  - [ ] Crea el código del impuesto "IGT" y asignar el tipo de impuesto IGTF Venezuela
  - [ ] Crear la vigencia de impuesto para el IGTF
    - [ ] Seleccionar en forma de calculo
      - [ ] Cliente porcentaje 3%
      - [ ] Proveedor porcentaje 3%

- [ ] ## Configurar documentos

  - [ ] Asignar en la definición del documento (ActDefDoc) el calculo del impuesto a los siguientes documentos de clientes
    - [ ] Factura de mostrador
    - [ ] Factura de crédito
    - [ ] Nota de crédito
    - [ ] Nota de debito
  - [ ] Asignar en la definición del documento (ActDefDoc) el calculo del impuesto a los siguientes documentos de proveedor
    - [ ] Factura de mostrador
    - [ ] Factura de crédito
    - [ ] Nota de crédito
    - [ ] Nota de debito

- [ ] ## Registro de operaciones

  - [ ] ### **Ventas** 

    - [ ] #### Facturas  contado

      - [ ] Se debe registrar een las formas de pago el monto  en dólares  usdo para la cancelación de la deuda ya sea en efectivo o transferencia. 
      - [ ] Al presionar F8 se desplegara automáticamente el IGTF, si esta asignado el calculo en la definición
      
    - [ ] #### Facturas  crédito
      
      El Calculo del impuesto es manual ya que este dependerá del convenio o acuerdo de pago a realizar con el cliente . Se debe acordar la cantidad de divisas y la tasa. 
  
      - [ ] ##### Acordadas
  
        Si conocemos el monto a cancelar en divisas se puede crear  impuesto en la factura de crédito antes de presionar F8. Con el monto gravado correspondiente a la cantidad de divisas multiplicada por su tasa en moneda nacional. Esto ajustara el total del documento .
      
      - [ ] ##### No acordadas
      
        Cuando la factura no es cancelada de la forma acordada y se presenta un pago en divisas no esperado se debe:
      
        Realizar una nota de debito por el monto de la diferencia que solo incluya el impuesto a  cancelar al momento del pago (IGTF  ) y aplicarlo a la factura
      
      - [ ] ### Compras

    - [ ] #### Facturas  crédito

      El Calculo del impuesto es manual ya que este dependerá del convenio o acuerdo de pago a realizar con el proveedor . Se debe acordar la cantidad de divisas y la tasa. 

      - [ ] ##### Acordadas

        Si conocemos el monto a cancelar en divisas se puede crear el   impuesto en la factura de crédito antes de presionar F8. 

        Una vez posicionado en la grilla , presionar Ctrl+I o solo I y podrá agregar el impuesto con el monto gravado correspondiente a la cantidad de divisas multiplicada por su tasa en moneda nacional se debe cargar los siguientes datos:

        - [ ] Impuesto: IGT
        - [ ] % impuesto: 3.00
        - [ ] Subtotal Gravado: 1000
        - [ ] Subtotal Impuesto: 30.00
  
      - [ ] ##### No acordadas
  
        Cuando la factura no es cancelada de la forma acordada y se presenta un pago en divisas no esperado se debe:
  
        Realizar una nota de debito por el monto de la diferencia que solo incluya el impuesto a  cancelar al momento del pago (IGTF  ) y aplicarlo a la factura
  
        Una vez posicionado en la grilla , presionar Ctrl+I o solo I y podrá agregar el impuesto con el monto gravado correspondiente a la cantidad de divisas multiplicada por su tasa en moneda nacional se debe cargar los siguientes datos:
  
        - [ ] Impuesto: IGT
        - [ ] % impuesto: 3.00
        - [ ] Subtotal Gravado: 1000
        - [ ] Subtotal Impuesto: 30.00
  
    
  
  ## Configurar Reportes
  
  - [ ] ### Libro de ventas
  
    - [ ] Acceso rápido RepLbrVta
    - [ ] Ir a la pestaña Ventas
    - [ ] Tildar la opción de Mostrar Oros Impuestos y aparecerá una columna a la derecha del reporte mostrando los montos del iGTF calculado por factura y su respectivo subtotal,
  
  - [ ] ### Libro de compras
  
    - [ ] Acceso rápido RepLbrCmp
    - [ ] Ir a la pestaña Compras
    - [ ] Tildar la opción de Mostrar Oros Impuestos y aparecerá una columna a la derecha del reporte mostrando los montos del iGTF calculado por factura y su respectivo subtotal,
  
  - [ ] ### Libro de IGTF
  
    - [ ] Se debe agregar el Tool    GEVT_RepImtIGTF
    - [ ] acceso rápido RepImtIGTF