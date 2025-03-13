# Constrained Device Application (Connected Devices)

## Lab Module 03

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Se habilitó la función de simular sensores y actuadores. Para gestionar la información relacionada con estos dispositivos, se desarrollaron clases específicas. Se introducen managers que se encargan de supervisar y controlar tanto los sensores como los actuadores. Hay un manager principal que coordina dichos managers. 

How does your implementation work?

Los sensores y actuadores heredan de las clases BaseActuatorSimTask y BaseSensorSimTask, que les permiten generar datos mediante las clases ActuatorData y SensorData. Los actuadores derivados de BaseActuatorSimTask son HumidifierActuatorSimTask y HvacActuatorSimTask, mientras que los sensores derivados de BaseSensorSimTask son HumiditySensorSimTask, PressureSensorSimTask y TemperatureSensorSimTask. Los sensores simulados generan datos de manera periódica gracias al SensorAdapterManager, y los actuadores son gestionados por el ActuatorAdapterManager. Todos estos gestores, junto con el SystemPerformanceManager, son supervisados por el DeviceDataManager.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Python/tree/lab03

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ActuatorDataTest
- SensorDataTest
- SystemPerformanceDataTest
- HumiditySensorSimTaskTest
- PressureSensorSimTaskTest
- TemperatureSensorSimTaskTest
- HumidifierActuatorSimTaskTest
- HvacActuatorSimTaskTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- ConstrainedDeviceAppTest
- DeviceDataManagerNoCommsTest

EOF.
