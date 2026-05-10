# WebConfig

**ESP32 Web Configuration Portal with NVS Persistent Storage**

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Work%20In%20Progress-yellow.svg)]()
[![ESP32](https://img.shields.io/badge/ESP32-Arduino%20Core%202.x%2F3.x-red.svg)](https://github.com/espressif/arduino-esp32)

---

WebConfig is a universal ESP32 Arduino library that provides a web-based configuration portal. Activate it by pulling a GPIO pin HIGH — the library starts a WiFi hotspot and serves a mobile-friendly web interface where users can configure and save parameters to non-volatile storage (NVS). All settings survive reboots and power cycles.

> 🚧 **This library is currently under development. Stay tuned!**

---

## Planned Features

- **GPIO pin activation** — config mode activates while pin is held HIGH, with built-in debounce
- **Automatic SSID & password** — generated from device MAC address, unique per device
- **Captive portal** — phone automatically opens config page when connecting to hotspot
- **6 parameter types** — text, integer, float, boolean, password (plain & encrypted), dropdown
- **Parameter groups** — organize parameters into labeled sections
- **Dual validation** — client-side (JavaScript) and server-side (ESP32) validation
- **NVS persistent storage** — settings survive reboots and power loss
- **Status system** — polling and callback
- **Log system** — indexed log entries, auto-cleared on config mode exit
- **Session management** — MAC-based single-client sessions
- **Fully localizable** — every visible text and error message is user-definable
- **Programmatic access** — read and write parameters anytime
- **Mobile-friendly UI** — responsive design
- **Arduino IDE 2.0+ & PlatformIO** — both supported

---

## Hardware Compatibility

**Supported:** ESP32, ESP32-S2, ESP32-S3, ESP32-C3, ESP32-C6  
**Not supported:** ESP32-H2 (no WiFi)

---

## License

Copyright (c) 2024 [arvismastins](https://github.com/arvismastins)

Licensed under the [Apache License 2.0](LICENSE).
