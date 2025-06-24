# Predicción de Cancelación de Clientes en Telecom Interconnect

## 1. Descripción del proyecto

El presente proyecto, para la compañía de telecomunicaciones Interconnect, se centra en una tarea de clasificación para predecir la cancelación de clientes, con el fin de retener a estos clientes a través de ofrecimiento de códigos promocionales y opciones de planes especiales. En general en los negocios resulta más económico retener clientes que atraer nuevos clientes, por lo que este proyecto será de gran valor para la compañía.

El equipo de marketing ha recopilado algunos datos de sus clientes, incluyendo información sobre sus planes y contratos. A continuación se describen los servicios que ofrece la compañía y la descripción de los datos proporcionados.

### 1.1 Servicio de Interconnect

Interconnect proporciona principalmente dos tipos de servicios:

1. Comunicación por teléfono fijo. El teléfono se puede conectar a varias líneas de manera simultánea.
2. Internet. La red se puede configurar a través de una línea telefónica (DSL, *línea de abonado digital*) o a través de un cable de fibra óptica.

Algunos otros servicios que ofrece la empresa incluyen:

- Seguridad en Internet: software antivirus (*Protección De Dispositivo*) y un bloqueador de sitios web maliciosos (*Seguridad En Línea*).
- Una línea de soporte técnico (*Soporte Técnico*).
- Almacenamiento de archivos en la nube y backup de datos (*Backup On line*).
- Streaming de TV (*Streaming TV*) y directorio de películas (*Streaming Películas*)

La clientela puede elegir entre un pago mensual o firmar un contrato de 1 o 2 años. Puede utilizar varios métodos de pago y recibir una factura electrónica después de una transacción.

### 1.2 Descripción de los datos

Los datos consisten en archivos obtenidos de diferentes fuentes:

- `contract.csv` — información del contrato;
- `personal.csv` — datos personales del cliente;
- `internet.csv` — información sobre los servicios de Internet;
- `phone.csv` — información sobre los servicios telefónicos.

En cada archivo, la columna `customerID` (ID de cliente) contiene un código único asignado a cada cliente. La información del contrato es válida a partir del 1 de febrero de 2020.

### 1.3 Objetivo

El objetivo de este proyecto es crear un modelo de aprendizaje automático que, con base en la información histórica proporcionada por la compañía, sea capaz de predecir cuáles son los clientes que pudieran estar próximos a cancelar los servicios que tienen contratados con la compañía. Para ello se utilizará como variable objetivo la información que tiene la compañía sobre las personas que ya han cancelado su servicio, con ello podremos hacer una clasificación correcta y descubrir los patrones que llevan a los clientes a cancelar sus servicios.