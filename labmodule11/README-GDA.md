# Gateway Device Application (Connected Devices)

## Lab Module 11

Be sure to implement all the PIOT-GDA-* issues (requirements) listed.

### Description

NOTE: Include two full paragraphs describing your implementation approach by answering the questions listed below.

What does your implementation do? 

La implementación recibe mensajes por MQTT y lo sube al cloud de Ubidots. La información que se envia es la de activación del actuador LED, la utilización de memoria y CPU, la temperatura y la humedad.

How does your implementation work?

En MqttClientConnector añadimos las funcionalidades para conectarse al cloud. Se modifica el json recibido por Mqtt para que cumpla con el estandar de ubidots.

### Code Repository and Branch

NOTE: Be sure to include the branch.

URL: https://github.com/Barandelaa/PIC_Java/tree/lab11


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

- MqttClientConnectorTest
- CloudClientConnectorTest
- 

EOF.

Información de los sensores (ignorar el sensor de luz ya que es de una rama posterior):
![image](https://github.com/user-attachments/assets/32480674-47c8-4f98-a65e-4c34860c079f)

Ejemplo de como se ve la información de los sensores:
![image](https://github.com/user-attachments/assets/e8dfa356-2e52-47b5-b5b7-dcaa44f4371e)

Mensaje del actuador:
![image](https://github.com/user-attachments/assets/5c21798f-3c91-4925-9459-cd42ca449e5c)


