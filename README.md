# RESTful ESP32 Sensor and Control Network

This project creates a network of **ESP32-based smart sensors and controllers**, each exposing a **RESTful API**. These devices collect data from sensors, control actuators like LEDs or servo motors, and provide a flexible interface for remote monitoring and control.

## Key Features

* **Web Server**: Each ESP32 device runs a web server using the **ESP-IDF framework**.
* **RESTful API**: Easy integration and communication via REST endpoints.
* **Actuator Control**: APIs to control LEDs, servo motors, etc.
* **Sensor Data Access**: Endpoints to retrieve live sensor data.
* **Modular Design**: Clean separation of headers and source files for scalability.
* **Expandable**: Easily add new sensors, actuators, or additional ESP32 nodes.

## Project Goals

* **Scalable and Flexible** platform for remote monitoring and control.
* **Maintainable Codebase** using best practices in code organization and modular design.
* **Thorough Documentation** to support future development and open collaboration.

## Project Structure (planned)

```
esp32_rest_network/
├── components/
│   ├── sensor_driver/
│   ├── actuator_driver/
│   └── rest_api/
├── main/
│   ├── app_main.c
│   └── ...
├── include/
│   ├── sensor_driver.h
│   └── actuator_driver.h
├── CMakeLists.txt
└── README.md
```

## In Progress

* [ ] RESTful API design for `/sensors` and `/actuators`
* [ ] Modular hardware abstraction layer
* [ ] Example demo for LED control and temperature sensing

## Tools and Frameworks

* [ESP-IDF](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/)
* RESTful HTTP Server via `esp_http_server.h`
* JSON support via `cJSON` or equivalent

## Documentation Goals

* Setup and flash instructions
* REST API reference
* Hardware integration guide

---

