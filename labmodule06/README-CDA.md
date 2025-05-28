# Constrained Device Application (Connected Devices)

## Lab Module 06

Be sure to implement all the PIOT-CDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 
Se ha añadido la funcionalidad de conexión para el cliente, permitiéndole suscribirse y publicara distintos topics.

How does your implementation work?
Casi toda la funcionalidad tiene lugar en el MqttClientConnector. El DeviceDataManager usa la clase anterior para conectarse y suscribirse al topic.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Python/tree/lab06


### Unit Tests Executed

NOTE: The instructor will execute your unit tests. You only need to list each test case below
(e.g. ConfigUtilTest, DataUtilTest, etc). Be sure to include all previous tests, too,
since you need to ensure you haven't introduced regressions.

- 
- 
- 

### Integration Tests Executed

NOTE: The instructor will execute most of your integration tests using their own environment, with
some exceptions (such as your cloud connectivity tests). In such cases, they'll review
your code to ensure it's correct. As for the tests you execute, you only need to list each
test case below (e.g. SensorSimAdapterManagerTest, DeviceDataManagerTest, etc.)

- MqttClientControlPacketTest
- MqttClientConnectorTest
-
Wireshark (MqttClientConnectorTest):
![imaxe](https://github.com/user-attachments/assets/157f8762-cf1b-465f-9570-6658b2a6ae81)

Wireshark (MqttClientControlPacketTest):
![imaxe](https://github.com/user-attachments/assets/6b5a99e4-6edb-40e2-80d0-d6c3a856347c)


