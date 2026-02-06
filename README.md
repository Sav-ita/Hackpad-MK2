# Hackpad MK2

A premium, 9-key custom macro pad based on the RP2040 microcontroller, featuring an SSD1306 OLED display for real-time feedback.

![Hackpad MK2](Images/hackpad.jpg) *(Note: Ensure an image exists in the Images folder)*

## Features

- **9 Programmable Keys**: Full control over your shortcuts and macros.
- **RP2040 Powered**: High-performance, dual-core ARM Cortex-M0+ processor.
- **OLED Display**: 128x32 SSD1306 display to show key presses and status.
- **CircuitPython**: Easy to customize and flash without complex IDEs.
- **3D Printed Case**: Sleek, functional design with top and bottom shells.

## Repository Structure

- `/CAD`: 3D models and assembly files for the case (STEP format).
- `/PCB`: KiCad design files, including schematic and PCB layout.
- `/Firmware`: CircuitPython source code (`main.py`).
- `/Images`: Project photos and diagrams.

## Hardware Specifications

- **Controller**: RP2040 (e.g., Raspberry Pi Pico or similar module).
- **Display**: 128x32 I2C OLED (SSD1306).
- **Matrix**: 9 independent keys pulled up to internal resistors.
- **Interface**: USB HID (Keyboard).

## Software Setup

1. Flash your RP2040 with the latest [CircuitPython firmware](https://circuitpython.org/downloads).
2. Copy the contents of the `/Firmware` folder to the `CIRCUITPY` drive.
3. Ensure the following libraries are present in the `lib` folder on the device:
   - `adafruit_display_text`
   - `adafruit_ssd1306`
   - `adafruit_hid`

## Customization

The `key_map` in `main.py` allows you to redefine what each key does. Simply modify the `Keycode` values to match your preferred shortcuts.

---

**Designed and Programmed by Saverio Martino**
