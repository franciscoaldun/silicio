# Silicio

**English** · [Español](README.es.md)

**Electronics and computers, from the transistor up.** A Windows simulator where everything is made of transistors working live, and where you can zoom into any chip until you see them switch.

[![Condor, an 8-bit computer made of 6,609 transistors](capturas/condor.jpg)](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-video-condor.mp4)

▶ **[Watch the video (64 s)](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-video-condor.mp4)** · ⬇ **[Free trial](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-1.0.1-prueba.zip)** · 🛒 **[Full version on the Microsoft Store](https://apps.microsoft.com/detail/9PFK8C3LC5NB)**

## What it is

In Silicio the basic part is the transistor. Gates, flip-flops, counters, memories and chips are built from N and P transistors, and a SPICE-like analog engine handles LEDs, diodes, transistors, capacitors, inductors and quartz crystals. You build on a schematic, on a breadboard like the real one, or in a free-wiring mode, and with the **infinite zoom** you dive into any block or chip to watch it work inside, on the same canvas, without opening windows.

It is made for learning electricity, electronics, digital systems and computer architecture by seeing how everything really works, from an LED to a whole computer. It works offline, in English and Spanish.

## What you can do

### Condor: an 8-bit computer made of transistors
6,609 transistors with a CPU, ROM, RAM, clock, switches and displays, all connected with real wires. It runs the Fibonacci sequence and four other programs, and you can zoom from the board down to every transistor while it runs.

### Infinite zoom and microscope
Zoom into a block and its circuit appears inside, working: from the clock to the divider, from the divider to the flip-flop, from the flip-flop to the NAND gate, and from the NAND to its 4 transistors. With the **microscope**, each chip looks like fabricated silicon, with its pads, power rings, transistors and three metal layers lit up live, and the "Fabricate layer by layer" button builds it step by step.

![Infinite zoom inside the frequency divider](capturas/zoom-infinito.jpg)

### A breadboard with chips you can open
Resistors with their color bands, LEDs, push buttons, potentiometers, transistors, relays, sensors, motors and **39 DIP chips**: 74HC logic made of CMOS transistors, counters, shift registers, the 555, op-amps, I2C memories and clocks. Parts burn out like in real life, and Silicio warns you about short circuits, reversed LEDs and floating pins. When your circuit works, you can turn it into a **printed circuit board in KiCad**.

![Breadboard with a 74HC00 chip](capturas/protoboard-74hc00.jpg)

### ESP32-C3 and Arduino Uno running real programs
Write your program in C, press F9 and it runs on the simulated microcontroller: an ESP32-C3 (RISC-V) and an Arduino Uno R3 (ATmega328P), with a serial monitor. OLED, LCD, TM1637 and MAX7219 displays and HC-SR04, DHT22, DS18B20 and DS3231 sensors get the real protocol, bit by bit.

![ESP32-C3 with displays](capturas/esp32-pantallas.jpg)

### Lab instruments
Multimeter with diode mode, 4-channel oscilloscope with trigger, measurements and FFT, logic analyzer that decodes I2C, SPI and UART, function generator and current-limited power supply.

![Function generator, oscilloscope and multimeter](capturas/instrumentos.jpg)

### Offline datasheets, and Verilog
Every chip and part explains what it is used for in real life, what each pin does and how to connect it. And if you write a circuit in Verilog, Silicio turns it into gates made of transistors.

![Datasheet of the 74HC595](capturas/hoja-de-datos.jpg)

## Free trial

- Download [`Silicio-1.0.1-prueba.zip`](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-1.0.1-prueba.zip), unzip it and open `silicio.exe`. In the trial everything works, but you can't save or export projects. The first time it opens, it asks for your language (English or Spanish).
- **Requirements:** Windows 10 or 11, 64-bit, any x86-64 processor (Celeron and Pentium too). No internet needed.
- Windows may show "Windows protected your PC" because the program is new: "More info" → "Run anyway".

## Buy

**The full Silicio** saves your projects, exports images and KiCad boards, and every purchase helps it keep growing.

👉 **[Silicio on the Microsoft Store](https://apps.microsoft.com/detail/9PFK8C3LC5NB)**

You can also get there from the trial with the "Buy Silicio" button.

## Schools, universities and companies

Silicio works for classes in electricity, electronics, digital systems and computer architecture, and it runs offline in computer labs. Institutions and companies need an institutional license: write to **contacto@franciscoaldunate.cl**.

## License

Silicio is not free software: it is a program with all rights reserved, with a [license of use](LICENCIA.md) (in Spanish) that lets you use it to learn, study and make your own projects. What you create with Silicio is yours. Third-party components keep their licenses ([TERCEROS.md](TERCEROS.md)). Silicio does not collect data ([PRIVACIDAD.md](PRIVACIDAD.md)).

## Versions

| Version | Date | File | SHA-256 |
|---|---|---|---|
| 1.0.1 | 2026-11-10 | `Silicio-1.0.1.msix` (full, Microsoft Store) | `851072fab8eaee1ec8c7c453be52d5228f7edd0cf361be1b3b6f352f5c427cba` |
| 1.0.1 | 2026-11-11 | `Silicio-1.0.1-prueba.zip` (trial) | `f3babfad58d1fe413386aa85ce0b1d842ecc82bd598303fd1bdda2d46edea8da` |
| 0.6.1 | 2026-10-18 | `Silicio-0.6.1-portable.zip` (first public edition) | `36c89bb2b099ccfecb7f0a4fe93e2aeaab3d149166abd6f62a28e85d55895815` |

Technical description and dated record on Zenodo: version 1.0.1, [10.5281/zenodo.24134452](https://doi.org/10.5281/zenodo.24134452); version 0.6.1, [10.5281/zenodo.23460025](https://doi.org/10.5281/zenodo.23460025).

The changes in each version are in [CAMBIOS.md](CAMBIOS.md) (in Spanish).

---

Made by Francisco Aldunate · [contacto@franciscoaldunate.cl](mailto:contacto@franciscoaldunate.cl)
