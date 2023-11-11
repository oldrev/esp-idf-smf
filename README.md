# State Machine Framework for ESP-IDF

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

## Overview

This repository contains a port of the Zephyr Real-Time Operating System (RTOS) State Machine Framework to the ESP-IDF framework. The State Machine Framework provides a flexible and efficient way to implement state machines in your ESP-IDF projects.

## Features

- Easy integration with ESP-IDF projects as a Component.
- Utilizes the powerful Zephyr State Machine Framework for efficient state management.
- Apache 2.0 licensed for open-source use.

## Getting Started

To use the ESP-IDF Zephyr State Machine Framework in your project, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/oldrev/esp-idf-smf.git
    ```

2. Add the component to your ESP-IDF project:

    ```bash
    cd your-espidf-project
    mkdir components
    cp -r path/to/esp-idf-smf components/
    ```

    Don't forget to add the `smf` requirement to your project's `CMakeLists.txt` file.

3. Include the State Machine Framework header in your code:

    ```c
    #include "smf/smf.h"
    ```

4. Add the following line to your project's `sdkconfig` file to enable support for multi-level state machines:
    ```plaintext
    CONFIG_SMF_ANCESTOR_SUPPORT=y
    ```

5. Start using the State Machine Framework in your project.


## Example Usage

To integrate the Zephyr State Machine Framework into your ESP-IDF project, you can refer to the official Zephyr RTOS documentation for the State Machine Framework: [Zephyr SMF Documentation](https://docs.zephyrproject.org/latest/services/smf/index.html).

The integration process is similar to the standard Zephyr workflow, with the additional step of including this component in your ESP-IDF project. Once the component is added, you can follow the Zephyr documentation for creating and managing state machines.

## License

This project is licensed under the Apache License 2.0 - see the LICENSE file for details.

## Acknowledgments

This project is built upon the Zephyr Real-Time Operating System and ESP-IDF.

Thanks to the open-source community for their contributions.
