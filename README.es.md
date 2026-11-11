# silicio

[english](README.md) · **español**

hola, soy francisco, de chile. silicio es un simulador de circuitos que estoy haciendo desde octubre donde todo esta hecho de transistores, y te puedes acercar a cualquier chip hasta verlos conmutar. es como hacer zoom en google earth pero adentro de una cpu, esa fue la idea desde el primer dia.

[![cóndor, una computadora de 8 bits hecha de 6.609 transistores](capturas/condor.jpg)](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-video-condor.mp4)

[ver el video (64 s)](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-video-condor.mp4) · [probar gratis](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-1.0.1-prueba.zip) · [versión completa en la microsoft store](https://apps.microsoft.com/detail/9PFK8C3LC5NB)

## que hace

lo que más me enorgullece es cóndor, una computadora de 8 bits hecha de 6.609 transistores, unida con cables de verdad, corriendo fibonacci. te puedes acercar desde la placa a la cpu, de la cpu a las compuertas y de ahi a los transistores, y sigue funcionando en todos los niveles mientras la miras. tambien tiene un microscopio que muestra cada chip como silicio de verdad, con las capas de metal encendiéndose, y un botón que fabrica el chip capa por capa como en una fábrica.

![zoom dentro del divisor de frecuencia](capturas/zoom-infinito.jpg)

ademas sirve como protoboard normal. pones piezas reales (chips 74HC, el 555, amplificadores, pantallas lcd y oled, sensores, servos, 39 chips en total) y se portan como las de verdad: un led sin resistencia se quema, una entrada cmos al aire lee cualquier cosa, un chip sin gnd no funciona. cuando el circuito anda lo puedes exportar a kicad y hacer la placa de verdad.

![protoboard con un 74HC00](capturas/protoboard-74hc00.jpg)

trae un esp32-c3 y un arduino uno que corren código real. escribes en c, apretas F9 y se compila y corre dentro del chip simulado, con monitor serie. las pantallas y los sensores reciben el protocolo real bit por bit, asi que si tu i2c está malo, acá también.

![esp32-c3 con pantallas](capturas/esp32-pantallas.jpg)

tambien hay un pequeño laboratorio para medir todo: osciloscopio de 4 canales con fft, multímetro, analizador lógico que decodifica i2c, spi y uart, generador de funciones y fuente con límite de corriente.

![generador, osciloscopio y multímetro](capturas/instrumentos.jpg)

cada chip trae su hoja de datos adentro del programa, sin internet, y puedes escribir verilog y ver como se convierte en compuertas y transistores.

## pruébalo

baja [Silicio-1.0.1-prueba.zip](https://github.com/franciscoaldun/silicio/releases/download/v1.0.1/Silicio-1.0.1-prueba.zip), descomprímelo y abre `silicio.exe`. la prueba trae todo, solo que no guarda ni exporta, asi que cuando la cierras tu circuito se pierde. windows 10/11 de 64 bits, cualquier procesador (celeron tambien), sin internet, en español e inglés. lo más probable es que windows diga "windows protegió su pc" porque el programa es nuevo: "más información" → "ejecutar de todas formas".

si te gusta, la versión completa está en la [microsoft store](https://apps.microsoft.com/detail/9PFK8C3LC5NB). eso es lo que me deja seguir trabajando en esto.

## colegios

si haces clases de electrónica, sistemas digitales o arquitectura de computadores y lo quieres para una sala de computación, escríbeme a contacto@franciscoaldunate.cl. hay licencia para colegios y empresas.

## otras cosas

- no es código abierto, todos los derechos reservados ([licencia](LICENCIA.md)). lo que armes con silicio es tuyo.
- no recopila ningún dato ([privacidad](PRIVACIDAD.md)).
- lo de terceros está en [TERCEROS.md](TERCEROS.md) y los cambios de cada versión en [CAMBIOS.md](CAMBIOS.md).
- constancia con fecha de cada versión en zenodo: [1.0.1](https://doi.org/10.5281/zenodo.24134452) y [0.6.1](https://doi.org/10.5281/zenodo.23460025). las huellas sha-256 de cada archivo están en las [versiones](https://github.com/franciscoaldun/silicio/releases).

errores, ideas, lo que sea: abre un issue o escríbeme, leo todo.

francisco
