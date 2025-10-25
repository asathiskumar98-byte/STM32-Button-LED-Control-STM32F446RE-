# STM32 Button + LED Control (STM32F446RE)

This project demonstrates a simple **Button-controlled LED** using the **STM32F446RE** microcontroller with **HAL libraries** in STM32CubeIDE.

## 🧠 Description
- When the **User Button (PC13)** is pressed, the **LED (PA5)** turns ON.  
- When released, the LED turns OFF.  
- Debouncing is not implemented — this is a basic digital input/output example.

## ⚙️ Hardware Setup
| Pin | Function | Description |
|-----|-----------|--------------|
| PA5 | Output | LED (active HIGH) |
| PC13 | Input | Push button (active LOW) |

## 🧰 Tools Used
- STM32CubeIDE 1.x
- STM32CubeMX (for .ioc configuration)
- STM32F446RE Nucleo board

## 🚀 How to Build & Run
1. Open project in **STM32CubeIDE**  
2. Connect your **Nucleo board**  
3. Build → Debug → Run  
4. Press the button — the LED should toggle ON/OFF.

## 📂 File Overview
- **Core/Src/main.c** → main logic  
- **Core/Inc/main.h** → header definitions  
- **STM32_Button_LED.ioc** → pin, clock, and peripheral configuration  
- **Drivers/** → STM32 HAL driver files  
