````markdown
# Web-Controlled LED Matrix

A WiFi-controlled, web-based LED matrix designed for interactive climbing walls. This project uses an ESP-32 microcontroller to host a web server, allowing users to control an RGB LED grid embedded in a climbing wall from any browser-enabled device connected to the same network.

[A short video of the prototype in operation](https://youtu.be/ybT7Ar16RoI)

## Features

- **Web Interface:** Intuitive web control panel served directly from the ESP-32.
- **Customizable Patterns:** Select, create, or randomize climbing routes, challenges, or light patterns.
- **Real-Time Updates:** Instantly apply lighting changes from your phone or laptop.
- **Standalone Operation:** Once started, the ESP-32 acts as both the LED controller and the wireless access point or WiFi client.
- **Scalable:** Works for walls of various sizes by adjusting the code for your matrix dimensions.
- **Efficient Hardware:** Runs on a cost-effective ESP-32 and commercially available LED strips (WS2812/Neopixel or compatible).

## Project Overview

This project combines software, hardware, and firmware to create an interactive climbing experience. The ESP-32 hosts a responsive web application allowing climbers and coaches to:

- Highlight routes and holds for training or games
- Design custom lighting patterns/sequences
- Run challenges such as "find-the-hold" or timer-based bouldering exercises

## Hardware Requirements

- **ESP-32** development board
- **Addressable RGB LED strip** (e.g., WS2812/Neopixel), arranged in a matrix
- **Power supply** suitable for your LED count (e.g., 5V/10A for larger matrices)
- Wires, connectors, and optional casing

## Software Requirements

- [Arduino IDE](https://www.arduino.cc/en/software) or [PlatformIO](https://platformio.org/), with ESP-32 board support
- [FastLED](https://github.com/FastLED/FastLED) or [Adafruit NeoPixel](https://github.com/adafruit/Adafruit_NeoPixel) library
- [ESPAsyncWebServer](https://github.com/me-no-dev/ESPAsyncWebServer) for serving the UI
- Basic HTML/CSS/JavaScript for the control interface

## Getting Started

1. **Hardware Setup:**
   - Wire up your LED grid to the ESP-32.
   - Ensure you have an adequate power supply for the number of LEDs.

2. **Firmware:**
   - Clone this repository and open it in your development environment.
   - Install required libraries in the Arduino IDE or PlatformIO.
   - Edit the configuration section (WiFi credentials, LED pin, number of LEDs, matrix dimensions, etc.).
   - Upload the code to your ESP-32.

3. **Accessing the Control Panel:**
   - Connect your device to the ESP-32’s WiFi network (AP mode) or find its IP on your network.
   - Open a browser and navigate to the provided address.
   - Use the interface to control the climbing wall’s LEDs!

## Example Use Cases

- **Training:** Light up specific routes for drills.
- **Games:** Timed challenges and “tag-the-light” games.
- **Demonstrations:** Show animated patterns for events or showcases.

## Contributing

Feel free to fork this repository, implement new features, fix bugs, or submit suggestions via pull requests or issues.

## License

This project is licensed under the MIT License.

---

Made with 💡 and 🧗‍♂️ by [the-duckchild](https://github.com/the-duckchild)
````
