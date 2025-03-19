# Gateway Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación gestiona datos de actuadores, sensores y rendimiento del sistema, y los serializa a JSON para asegurar la compatibilidad entre plataformas. DeviceDataManager maneja conexiones como MQTT, CoAP y clientes en la nube, y procesa los mensajes de los dispositivos. Además, gestiona el rendimiento del sistema, como el uso de CPU y memoria.

Se integra DeviceDataManager en GatewayDeviceApp para manejar las conexiones y los datos del sistema, activando y deteniendo los componentes según la configuración. También se asegura de que los mensajes se pasen correctamente entre los componentes y delega la gestión del rendimiento y las conexiones a DeviceDataManager.

How does your implementation work?

La implementación funciona mediante la gestión de datos a través de diversas clases que representan diferentes tipos de información, como datos de actuadores, sensores y rendimiento del sistema. DeviceDataManager es el componente principal, que se encarga de manejar las conexiones y procesar los datos.

Cuando se inicia el sistema, DeviceDataManager lee las configuraciones del archivo correspondiente y habilita las conexiones necesarias, como MQTT, CoAP o el cliente en la nube. A través de su método startManager(), se activa el monitoreo del rendimiento del sistema mediante SystemPerformanceManager, que recoge información sobre el uso de la CPU, memoria y disco. Esta información se pasa a un listener configurado, que a su vez la procesa.

Los datos de actuadores y sensores son gestionados y procesados por los métodos correspondientes en DeviceDataManager, que los recibe, los analiza y los transmite según sea necesario. Finalmente, cuando se detiene el sistema, DeviceDataManager desactiva las conexiones y detiene el monitoreo del rendimiento con el método stopManager().

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Java/tree/lab05


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- DataUtilTest
- ActuatorDataTest
- SensorDataTest
- SystemPerformanceDataTest


### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- GatewayDeviceAppTest
- DeviceDataManagerNoCommsTest
- DataIntegrationTest
- SystemPerformanceManagerTest

EOF.
