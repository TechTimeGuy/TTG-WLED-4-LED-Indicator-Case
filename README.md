# TTG WLED 4-LED Indicator Case

A compact WLED-powered 4-LED status indicator designed for Home Assistant.
This project provides a simple, glanceable way to display Air Quality (AQI),
3D printer status, battery voltage, or any numeric sensor without dashboards
or screens.

## Repository Structure

TTG-WLED-4-LED-Indicator-Case/
- stl/        → 3D printable enclosure
- homeassistant/automation/blueprints/    → WLED / Home Assistant configuration
- docs/       → Quick Start & calibration documentation
- README.md
- .gitignore
- .gitattributes

## Features

- 4–5 LED visual indicator using the WLED Percent effect
- Works with any numeric Home Assistant sensor
- Calibration support for different LED counts
- Clean, desk-friendly 3D printed enclosure
- No cloud dependencies

## Requirements

- ESP32 (recommended)
- WLED installed on the ESP32
- 4–5 addressable LEDs (WS2812 / SK6812)
- Home Assistant with WLED integration
- FDM 3D printer (PLA or PETG recommended)

## 3D Printing

The enclosure files are located in the stl/ folder.

- No supports required
- Designed for standard FDM printers
- Snug friction fit for LEDs
- Print orientation: upright

## Setup Overview

1. Flash WLED onto your ESP32
2. Connect addressable LEDs to your chosen GPIO
3. Import the YAML from the esphome/ folder into Home Assistant
4. Select the sensor entity you want to display
5. Adjust calibration and thresholds as needed

Detailed calibration guidance is provided in the PDF.

## Documentation

See the docs/ folder for the Quick Start & Calibration Guide, including:
- Wiring reference
- LED calibration options
- Example Home Assistant sensor mappings

## Example Use Cases

- Air Quality (AQI / VOC / CO₂)
- 3D Printer status (Idle / Printing / Done / Error)
- Battery or solar voltage monitoring
- Temperature or humidity levels
- Any numeric Home Assistant entity

## Suggested GitHub Topics

esp32
home-assistant
esphome
wled
status-indicator
4-led
3d-printing
maker-project

## Notes

This project was designed to be simple, reliable, and flexible — ideal for
workshops, print rooms, and smart home setups where a screen isn’t needed.

Happy building.
