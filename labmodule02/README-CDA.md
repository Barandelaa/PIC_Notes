# Constrained Device Application (Connected Devices)

## Lab Module 02

Be sure to implement all the PIOT-CDA-* issues (requirements).

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Se puedo activar y parar el SystemPerformanceManager, que se ha conectado con el nucleo de la aplicación. Tabmien se ha implementado la base de las clases encargadas de recoger métricas de utilización de recursos (CPU y memoria) y se han conectado con el PerformanceManager para que sea capaz de controlarlas. 
How does your implementation work?
El PerformanceManager controla el SystemMemUtilTask y el SystemCpuUtilTask para monitorear la utilización de los recursos. Las dos clases mencionadas heredan de BaseSystemUtilTask que es la base para las clases de monitorización.
### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Python/tree/lab02

### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- ConfigUtilTest
- SystemCpuUtilTaskTest
- SystemMenmUtilTaskTest

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- ConstrainedDeviceAppTest
- SystemPerformanceManagerTest
- SystemPerformanceManagerTest

EOF.
