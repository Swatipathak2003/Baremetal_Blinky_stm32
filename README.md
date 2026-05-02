# 🔵 STM32 Bare-Metal LED Blink
### Black Pill · STM32F401CCU6 · No HAL · Direct Register Access

![Platform](https://img.shields.io/badge/Platform-STM32F401CCU6-blue)
![Type](https://img.shields.io/badge/Type-Bare--Metal-teal)
![Language](https://img.shields.io/badge/Language-C-green)
![HAL](https://img.shields.io/badge/HAL-None-red)

---

## 📌 Overview

Demonstrates LED blinking on the **STM32F401CCU6 (Black Pill)** using bare-metal programming — direct register access without HAL or any abstraction libraries.

---

## ⚙️ Hardware

| Component | Details |
|-----------|---------|
| MCU | STM32F401CCU6 (Black Pill) |
| LED | Onboard LED (GPIO-connected) |

---

## 🛠️ Concepts Used

| Category | Concepts |
|----------|----------|
| Core | Register-level programming, RCC clock configuration |
| Techniques | GPIO configuration, Bit manipulation |

---

## 🚀 How It Works

1. **Enable GPIO clock** — via the RCC peripheral register
2. **Configure GPIO pin** — set as push-pull output
3. **Toggle LED** — using a software delay loop

---

## 📂 Project Structure

```
├── main.c          # Application logic — clock init, GPIO config, blink loop
├── startup.s       # Reset handler, vector table, stack setup
├── linker.ld       # Memory layout — Flash and SRAM region mapping
└── images/
    ├── led_off.jpeg
    └── led_on.jpeg
```

---

## 📸 Output

> Onboard LED toggling — captured live on the Black Pill board.

| LED OFF | LED ON |
|:-------:|:------:|
| ![LED OFF](images/led_off.jpeg) | ![LED ON](images/led_on.jpeg) |

---

## 🎯 Learning Outcomes

- Understanding microcontroller peripheral registers
- Direct hardware control without HAL abstraction
- Fundamentals of embedded firmware development

---

## 👩‍💻 Author

**Swati Pathak**
