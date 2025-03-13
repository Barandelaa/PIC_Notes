# Constrained Device Application (Connected Devices)

## Lab Module 04

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Esta implementación simula sensores y actuadores como humidificadores, HVAC, pantallas LED, y sensores de temperatura, presión y humedad utilizando el Sense HAT, sin necesidad de hardware físico. Los sensores emulan datos ambientales y los actuadores se controlan mediante la pantalla del Sense HAT. La emulación se habilita mediante una configuración, y los sensores y actuadores se cargan dinámicamente usando importlib solo si la emulación está activada. Si no, se usan tareas simuladas. La estructura basada en herencia facilita la adición de nuevos sensores o actuadores al sistema.

How does your implementation work?

La implementación simula sensores y actuadores mediante clases como TemperatureSensorEmulatorTask, HumiditySensorEmulatorTask y HvacEmulatorTask. Si la emulación está habilitada (self.useEmulator = True), las clases se cargan dinámicamente con importlib. Si no, se usan clases simuladas que generan datos. Las funciones self._initEnvironmentalSensorTasks() y self._initEnvironmentalActuationTasks() gestionan la inicialización de sensores y actuadores, permitiendo integrar fácilmente nuevos dispositivos sin modificar el código existente.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Python/tree/lab04


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- SenseHatEmulatorQuickTest.py
- HumidifierEmulatorTaskTest.py
- HvacEmulatorTaskTest.py
- LedDisplayEmulatorTaskTest.py
- HumidityEmulatorTaskTest.py
- PressureEmulatorTaskTest.py
- TemperatureEmulatorTaskTest.py

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- ActuatorEmulatorManagerTest.py
- SensorEmulatorManagerTest.py
- 

EOF.
