# ESP32-C3 BLE Mesh Remote

## Overview

The **ESP32-C3 BLE Mesh Remote** is a highly compact and low-power remote control device built around the **ESP32-C3** microcontroller. The system features 4 user input buttons, an RGB5050 LED, and runs on a **CR2032 battery**. It only activates when a button is pressed, ensuring minimal power consumption. The device supports **Bluetooth Low Energy (BLE)**, **BLE Mesh**, **Wi-Fi**, and **ESP-NOW** protocols for efficient data transmission.

The design is optimized for low-power operation, making it ideal for battery-powered remote control applications. It’s capable of communicating with other devices in a BLE Mesh network, making it perfect for IoT and home automation solutions.

![Front View](https://github.com/karthirilla/ESP32_BLE_Mesh_Remote/blob/main/ESP32_HOME_AUTOMATION_BLE_MESH_REMOTE_FRONT.png)
![Back View](https://github.com/karthirilla/ESP32_BLE_Mesh_Remote/blob/main/ESP32_HOME_AUTOMATION_BLE_MESH_REMOTE_BACK.png)
![Front View](https://github.com/karthirilla/ESP32_BLE_Mesh_Remote/blob/main/ESP32_HOME_AUTOMATION_BLE_MESH_REMOTE_FRONT_1.png)

### Key Features

- **Low Power Consumption**: The device only runs when a button is pressed, using minimal energy to extend battery life.
- **User Input**: 4 user input buttons for controlling various actions or devices.
- **RGB5050 LED**: Used for providing visual feedback on the device's status, Wi-Fi/BLE connection, and error indications.
- **Power Supply**: Runs on a **CR2032** coin cell battery.
- **Communication Protocols**:
  - **BLE**: Allows for local control and communication with other BLE-enabled devices.
  - **BLE Mesh**: Extends the communication range and creates a mesh network for communication between multiple devices.
  - **Wi-Fi**: Enables cloud connectivity and remote communication.
  - **ESP-NOW**: A peer-to-peer communication protocol for low-latency, low-power data transmission.
  
- **Compact and Lightweight**: The system is compact, lightweight, and portable, making it ideal for various remote control applications.
- **Arduino IDE and Espressif IDE**: Software is developed using both **Arduino IDE** and **Espressif IDE**, providing flexibility for different development environments.

## System Components

1. **ESP32-C3 Microcontroller**: The heart of the system, enabling Wi-Fi, BLE, ESP-NOW, and BLE Mesh communication.
2. **4 User Input Buttons**: Each button can trigger specific actions, such as sending commands or controlling devices in the BLE Mesh network.
3. **RGB5050 LED**: Provides visual feedback on the system's status (connected to BLE, Wi-Fi status, or error indication).
4. **CR2032 Battery**: A single **CR2032 coin cell** powers the device, offering a compact and long-lasting power source.
5. **Communication Protocols**:
   - **BLE** and **BLE Mesh**: For local control and communication in a networked environment.
   - **ESP-NOW**: For efficient, low-power peer-to-peer communication.
   - **Wi-Fi**: For connecting to the cloud or other devices over the internet.

## Features in Detail

### 1. **Low Power Operation**
- The ESP32-C3 microcontroller operates in **deep sleep mode** when not actively in use, and it only powers up when a button is pressed.
- The device automatically disconnects from the power supply when idle, ensuring minimal energy consumption and maximizing battery life.

### 2. **User Input Buttons**
- The device has **4 buttons** that can be programmed to perform specific actions.
- Each button press triggers the microcontroller to wake up and perform a task, such as sending data via BLE, controlling other devices in the BLE Mesh network, or communicating over Wi-Fi or ESP-NOW.

### 3. **RGB5050 LED**
- The **RGB5050 LED** provides real-time feedback about the system:
  - **Connection Status**: Displays different colors to indicate BLE or Wi-Fi connection status.
  - **Error Indication**: Blinks red to signal an error or failure in communication.
  - **Status Feedback**: Shows other statuses such as low battery or successful actions.

### 4. **BLE Mesh**
- The device supports **BLE Mesh**, allowing it to communicate with other BLE-enabled devices and form a mesh network. This extended communication range makes it suitable for large-scale IoT applications.
- **Mesh Networks**: Devices can relay messages to each other, ensuring coverage over a larger area.

### 5. **Wi-Fi and ESP-NOW**
- **Wi-Fi** support allows the remote to connect to the internet or communicate with other Wi-Fi-enabled devices.
- **ESP-NOW**: ESP32’s peer-to-peer communication protocol allows for low-latency data transmission between devices without requiring a central hub, making it ideal for direct device-to-device communication.

---

## Design and Development Process

### 1. **PCB Design**
The **PCB design** for the ESP32-C3-based remote was created using **EasyEDA**, ensuring a compact and optimized layout for low-power consumption and minimal space. The PCB design includes the following:
- ESP32-C3 microcontroller.
- Four buttons for user input.
- RGB5050 LED for visual feedback.
- Circuitry to support BLE Mesh, Wi-Fi, and ESP-NOW communication.
- Power management circuitry to ensure low power consumption using the CR2032 battery.

### 2. **PCB Assembly**
The assembly process was done manually, ensuring precise placement of the components to reduce power leakage and maintain low energy consumption. After assembly, the device was tested to verify its functionality and battery life.

### 3. **Software Development**
The software for the **ESP32-C3 BLE Mesh Remote** was developed using both **Arduino IDE** and **Espressif IDE**. Key software components include:
- **Button Handlers**: Code to handle the button presses and trigger actions.
- **Power Management**: Code for deep sleep and wake-up modes, allowing the device to only consume power when necessary.
- **Communication Protocols**: Code for **BLE**, **Wi-Fi**, and **ESP-NOW** communication, enabling the remote to connect to other devices, send data, and control systems remotely.
- **RGB5050 LED Feedback**: Code to control the RGB LED for status updates.

---

## Hardware Overview

- **Microcontroller**: ESP32-C3
- **Buttons**: 4 user input buttons for controlling actions.
- **RGB5050 LED**: RGB LED for status feedback.
- **Power Supply**: CR2032 coin cell battery (low power consumption).
- **Communication Modules**: BLE, BLE Mesh, ESP-NOW, and Wi-Fi.
- **PCB Design Tool**: EasyEDA

---

## Contributing

As this is a personal or internal project, contributions may not be accepted, but you're welcome to fork and adapt the project for your own use.

---

## License

This project is proprietary and not open-source.

---

## Acknowledgments

- **ESP32-C3**: Thanks to Espressif for providing the powerful ESP32-C3 microcontroller, which is perfect for low-power IoT applications.
- **EasyEDA**: For offering an accessible and user-friendly PCB design tool.
- **Arduino IDE & Espressif IDE**: For providing robust development environments for the ESP32-C3 platform.

---

## Additional Notes

- The **CR2032 battery** is chosen for its compact size and ability to provide long-lasting power with low power consumption. Depending on usage patterns, the battery can last several months to a year.
- The system is highly customizable, and additional features can be added, such as more input buttons, additional LEDs, or support for other IoT protocols.

---

## Conclusion

The **ESP32-C3 BLE Mesh Remote** is a compact and efficient solution for remote control applications in a BLE Mesh network. It is designed to be low power, using the CR2032 battery and waking up only when needed, making it an ideal choice for long-term, battery-powered IoT projects.

