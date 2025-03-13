# Constrained Device Application (Connected Devices)

## Lab Module 05

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación actualiza el sistema para convertir y gestionar datos entre objetos y su formato JSON. Se crean métodos para convertir diferentes tipos de datos a JSON y viceversa, facilitando la serialización y deserialización de la información. Además, se actualiza el manejo de datos de rendimiento del sistema, almacenando la información sobre el uso de CPU y memoria y enviándola a través de un sistema de escucha cuando se recibe nueva telemetría. Si se establece un listener, este recibe los datos de rendimiento del sistema cada vez que se generan.

How does your implementation work?

La implementación se divide en dos tareas principales. Primero, se actualiza la clase DataUtil para convertir los objetos ActuatorData, SensorData y SystemPerformanceData a JSON y viceversa. Esto se hace utilizando métodos que serializan y deserializan los objetos mediante la biblioteca JSON, apoyándose en la clase JsonDataEncoder para convertir objetos en diccionarios antes de convertirlos a JSON. Los métodos también manejan casos de datos vacíos y nulos y pueden procesar números decimales cuando es necesario.

En segundo lugar, la clase SystemPerformanceManager se modifica para que, al recibir telemetría, recopile los datos de rendimiento del sistema (como el uso de CPU y memoria) y los almacene en un objeto SystemPerformanceData. Si hay un IDataMessageListener configurado, se le notifica con el nuevo objeto de datos.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Python/tree/lab05


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- DataUtilTest
- 
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- SystemPerformanceManagerTest
- DataIntegrationTest
- 

EOF.
