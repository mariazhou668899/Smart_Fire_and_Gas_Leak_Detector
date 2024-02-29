# Smart Fire & Gas Leak Detector Alert System

1. Introduction of Project
1.1. Introduction
Develop a smart and efficient system to detect the presence of fire or gas leak in indoor environments by using
Esp32 and Azure IoT Central Could Service, and send email alert and sound alarm for relevant persons.
1.2. Function
– Send DHT22 temperature and humidity data to IoT Central
– Send MQ2 gas data (smoke, CO etc.) to IoT Central
– Visualize sensor’s data on IoT Central
– View Client device information
– Send command to control buzzer and led working or not working from IoT Central
– Send command to set alarm limit value about temperature from IoT Central
– Send command to set alarm limit value about gas from IoT Central
– Send Fire or Gas Leak Email Alert to users
– Store raw telemetry into Blob Storage
2. Novelty
– Use MQTT and Wifi to establish communication
a. #include <WiFi.h>
b. #include <mqtt_client.h>
– Use DHT22 and MQ2 Sensors to detect fire and gas leak based on Azure IoT Central and Esp32
– Others use only one sensor like MQ2
– Or based on Esp8266 and platforms, which are not real cloud service like Azure or AWS
– Use Azure IoT Central to send command to control buzzer and led
– Use Azure IoT Central to send command to set alarm limit values for temperature and gas
– Use Rules of IoT Central to send the Email Alert
– Use any published templates resource by changing template model id
– Automatically generate Template for device using device code
– Others assign their own created templates for a device on IoT Central while they create a device. It is very
easy, but not smart
