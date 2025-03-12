# STM32F103C8T6 Button-Controlled LED Blink

## 📌 Deskripsi
Proyek ini menggunakan **STM32F103C8T6 (Blue Pill)** untuk mengontrol LED menggunakan push button. Saat tombol ditekan, LED akan mati. Jika tombol dilepas, LED akan blinking.

## 🛠 Perangkat yang Dibutuhkan
- 🟦 STM32F103C8T6 (Blue Pill)
- 💡 LED dan Resistor 110 ohm
- 🔘 Push Button
- 🔌 ST-Link

## 🖥 Software yang Dibutuhkan
- 🏗 **Keil Uvision**
- ⚙ **STM32CubeMX**

## ⚙ Konfigurasi STM32CubeMX (IOC Setup)

1. **Buka STM32CubeMX** dan pilih **STM32F103C8T6** sebagai mikrokontroler.
2. **Konfigurasi Clock**
   - Pilih **HSE** sebagai sumber clock eksternal.
   - Aktifkan **PLL** dan set ke **72MHz**.
3. **Konfigurasi GPIO**
   - **PA5**: Output (untuk LED),
   - **PB3**: Input (untuk tombol),
4. **Konfigurasi USART2 (untuk debugging via Serial)**
   - Enable USART2 dengan setting asynchronus.
5. **Generate Code** dan buka proyek di **Keil Uvision**.

## 📂 Struktur Kode
```bash
📁 Project_Folder
 ├── Core/
 │   ├── Inc/         # Header Files
 │   ├── Src/         # Source Files
 │   ├── main.c       # Program utama
 │   ├── gpio.c       # Konfigurasi GPIO
 │   ├── usart.c      # Konfigurasi UART
 ├── Drivers/         # Driver STM32
 ├── STM32CubeMX.ioc  # File konfigurasi IOC
```

## 🚀 Cara Menggunakan
1. **Build dan Flash kode ke STM32** menggunakan Keil Uvision.
2. Tekan tombol **PB3**, LED pada **PA5** akan mati.
3. Lepaskan tombol, LED akan berkedip.

## 👨‍💻 Kontributor
✍ [mauldevrinz] - [studymaull7@gmail.com]

