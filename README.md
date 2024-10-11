# CAN Translator
The CANought CAN Translator will implement the service-side interfaces defined in the CANought CAN Translator project. 
This project will host a thin layer of code that will translate incoming MQTT messages from the client to standard J1939 and UDS messages, and vice versa.

```plaintext
+--------------------------+
|   CAN Translator Client  |
+--------------------------+
            |  
            | MQTT
            |
+--------------------------+
|      CAN Translator      |     <--- You are here
+--------------------------+
            |
            | J1939 and UDS
            |
+--------------------------+
|      CAN Interface       |
|      e.g. SocketCAN      |
+--------------------------+
