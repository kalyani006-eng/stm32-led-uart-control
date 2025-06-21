# STM32 LED UART Control

This project allows you to control an LED using UART commands (`LED ON`, `LED OFF`) on an STM32F103C8T6 board using HAL libraries.

## 🔧 Setup

- MCU: STM32F103C8T6 (Blue Pill)
- Tool: STM32CubeIDE
- Baud rate: 115200
- Commands via UART:
  - `LED ON` → Turns on onboard LED (PA5)
  - `LED OFF` → Turns off onboard LED

## 📁 Files

- `Core/` - Source files
- `Drivers/` - HAL libraries
- `.ioc` - STM32CubeMX project config

## 🧠 Notes

- UART uses USART2
- `HAL_UART_RxCpltCallback()` handles command parsing
