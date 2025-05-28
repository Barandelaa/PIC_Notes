# Gateway Device Application (Connected Devices)

## Lab Module 07

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

Se añade la capacidad de publicar y suscribirse a topics utilizando Mosquitto.

How does your implementation work?

La funcionalidad se implementa en MqttClientConnector y son utilizadas por el DeviceDataManager.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Java/tree/lab07


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

EOF.

Wireshark (ConnectorTest):
![imaxe](https://github.com/user-attachments/assets/e551779d-9d5c-4796-893e-897d2a7e3b74)

Wireshark (packetTest):
![imaxe](https://github.com/user-attachments/assets/bb8da551-f2a7-4204-b82c-9d8c8de49318)

