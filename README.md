# silicio

**english** · [español](README.es.md)

hi, i'm francisco, from chile. silicio is a circuit simulator i've been building since october where everything is made of transistors, and you can zoom into any chip until you see them switching. kind of like zooming into google earth, but inside a cpu. that was the whole idea from day one.

[![condor, an 8-bit computer made of 6,609 transistors](capturas/condor.jpg)](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-video-condor.mp4)

[watch the video (64 s)](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-video-condor.mp4) · [free trial](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-1.0.1-prueba.zip) · [full version on the microsoft store](https://apps.microsoft.com/detail/9PFK8C3LC5NB)

## what it does

the part i'm proudest of is condor, an 8-bit computer made of 6,609 transistors, connected with real wires, running fibonacci. you can zoom from the board into the cpu, then into the gates, then into the transistors, and it keeps running at every level while you look at it. there's also a microscope view that shows each chip like real silicon, with the metal layers lighting up, and a button that builds the chip layer by layer like in a fab.

![zooming into the frequency divider](capturas/zoom-infinito.jpg)

it also works as a normal breadboard. you put real parts (74HC chips, the 555, op amps, lcd and oled displays, sensors, servos, 39 chips in total) and they behave like the real ones: an led without a resistor burns, a floating cmos input reads garbage, a chip without gnd just doesn't work. when your circuit works you can export it to kicad and make an actual pcb.

![breadboard with a 74HC00](capturas/protoboard-74hc00.jpg)

there's an esp32-c3 and an arduino uno that run real code. you write c, press F9 and it compiles and runs inside the simulated chip, with a serial monitor. the displays and sensors get the real protocol bit by bit, so if your i2c is wrong, it's wrong here too.

![esp32-c3 with displays](capturas/esp32-pantallas.jpg)

there's also a small lab to measure everything: oscilloscope (4 channels, fft), multimeter, logic analyzer that decodes i2c, spi and uart, a function generator and a bench power supply with current limit.

![generator, oscilloscope and multimeter](capturas/instrumentos.jpg)

every chip has its datasheet inside the program, no internet needed, and you can write verilog and watch it turn into gates and transistors.

## try it

download [Silicio-1.0.1-prueba.zip](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-1.0.1-prueba.zip), unzip it and open `silicio.exe`. the trial has everything, it just can't save or export, so when you close it your circuit is gone. windows 10/11 64-bit, any cpu (celeron too), works offline, english and spanish. windows will probably say "windows protected your pc" because the program is new: "more info" → "run anyway".

if you like it, the full version is on the [microsoft store](https://apps.microsoft.com/detail/9PFK8C3LC5NB). that's what lets me keep working on this.

## schools

if you teach electronics, digital systems or computer architecture and want it for a computer lab, write me at contacto@franciscoaldunate.cl. there's a license for schools and companies.

## other stuff

- it's not open source, all rights reserved ([license](LICENCIA.md), in spanish). what you build with it is yours.
- it doesn't collect any data ([privacy](PRIVACIDAD.md)).
- third party stuff in [TERCEROS.md](TERCEROS.md), changes in [CAMBIOS.md](CAMBIOS.md) (spanish for now).
- dated record of each version on zenodo: [1.0.1](https://doi.org/10.5281/zenodo.24134452) and [0.6.1](https://doi.org/10.5281/zenodo.23460025). the sha-256 of every file is in the [releases](https://github.com/franciscoaldun/silicio/releases).

bugs, ideas, anything: open an issue or write me, i read everything.

francisco
