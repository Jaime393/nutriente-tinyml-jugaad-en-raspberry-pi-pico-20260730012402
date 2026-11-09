# Fuentes — TinyML Jugaad en Raspberry Pi Pico

Fecha de consulta de todas las fuentes: 9 de noviembre de 2026.

## Primarias

1. **Raspberry Pi — Documentación de la serie Pico**
   https://www.raspberrypi.com/documentation/microcontrollers/pico-series.html
   Afirma: el Pico usa RP2040 o RP2350; se programa con MicroPython, C o C++; no corre Linux ni admite almacenamiento extraíble; se programa flasheando binarios a la flash. Tabla de modelos: Pico/Pico H/Pico W/Pico WH con 264 KB de SRAM y 2 MB de flash.
2. **Raspberry Pi — Página del producto Pico 2**
   https://www.raspberrypi.com/products/raspberry-pi-pico-2/
   Afirma: RP2350, doble Cortex-M33 o doble Hazard3 RISC-V a 150 MHz, 520 KB de SRAM, 4 MB de flash QSPI, desde 5 USD; la serie Pico 2 seguirá en producción hasta al menos enero de 2040.
3. **Raspberry Pi — Hoja de datos del Pico (PDF oficial)**
   https://pip-assets.raspberrypi.com/categories/610-raspberry-pi-pico/documents/RP-008307-DS-2-pico-datasheet.pdf
   Afirma (sección 3.1, consumo en VBUS a 5 V): demo *Popcorn* media ~86,5 mA; modo BOOTSEL media ~9 mA; modo DORMANT 0,8 mA; modo SLEEP 1,3 mA. Son valores típicos medidos, no máximos garantizados.
4. **Warden, P. y Situnayake, D. — *TinyML: Machine Learning with TensorFlow Lite on Arduino and Ultra-Low-Power Microcontrollers* (O'Reilly, 16 dic 2019)**
   https://books.google.de/books?id=sB3mxQEACAAJ
   Afirma: el equipo de Google Assistant detecta palabras con un modelo de solo 14 KB; el libro guía la creación de proyectos TinyML paso a paso con Arduino y microcontroladores de ultra bajo consumo.
5. **David, R. et al. — "TensorFlow Lite Micro: Embedded Machine Learning on TinyML Systems", MLSys 2021, arXiv:2010.08678**
   https://arxiv.org/abs/2010.08678
   Afirma: TFLM es un framework abierto de inferencia para sistemas embebidos, de Google y la Universidad de Harvard; resuelve los requisitos de eficiencia y la fragmentación entre plataformas con un enfoque basado en intérprete.
6. **raspberrypi/pico-tflmicro (GitHub)**
   https://github.com/raspberrypi/pico-tflmicro
   Afirma (vía su README y la búsqueda de GitHub del 9-nov-2026): puerto de TensorFlow Lite Micro para el Pico; repositorio de solo lectura, generado automáticamente desde el repositorio maestro de TensorFlow; 753 estrellas. Incluye los ejemplos *hello_world*, *micro_speech*, *magic_wand* y *person_detection*.
7. **Edge Impulse — Documentación: Raspberry Pi Pico**
   https://docs.edgeimpulse.com/hardware/boards/raspberry-pi-pico
   Afirma: el RP2040 está totalmente soportado por Edge Impulse (muestreo de datos, construcción de modelos y despliegue desde el estudio); el firmware es abierto (`edgeimpulse/firmware-pi-rp2xxx`); el Pico no tiene sensores incorporados; los núcleos M0+ carecen de extensiones SIMD y de FPU, lo que eleva la latencia frente a un Cortex-M4F al mismo reloj.
8. **Arm — Tabla comparativa de procesadores Cortex-M**
   https://raw.githubusercontent.com/troyguo/ARM_documents/main/Arm%20Cortex-M%20Processor%20Comparison%20Table.pdf
   Afirma: unidad de coma flotante (FPU): No en Cortex-M0/M0+/M23/M3; opcional de precisión simple en M4/M33; el Cortex-M33 es el primero con FPU de precisión simple obligatoria. Extensiones DSP: No en M0/M0+.
9. **Radjou, N., Prabhu, J. y Ahuja, S. — *Jugaad Innovation: Think Frugal, Be Flexible, Generate Breakthrough Growth* (Jossey-Bass, 2012)**
   https://ssir.org/books/excerpts/entry/jugaad_innovation_think_frugal_be_flexible_generate_breakthrough_growth
   Afirma (extracto en Stanford Social Innovation Review): *jugaad* es una palabra coloquial hindi que significa "una solución ingeniosa; una solución improvisada nacida del ingenio y la astucia"; hacer más con menos; cuatro años de investigación con emprendedores rurales y empresas; seis principios (buscar la oportunidad en la adversidad, hacer más con menos, pensar y actuar con flexibilidad, mantenerlo simple, incluir el margen, seguir el corazón).
10. **Universidad de Cambridge — "A touch of frugal genius" (15 oct 2015)**
    https://www.cam.ac.uk/research/features/a-touch-of-frugal-genius
    Afirma: *jugaad* es una mentalidad — encontrar soluciones prácticas, ser emprendedor con los recursos, aprender de la flexibilidad y la frugalidad; enfoque de abajo arriba basado en la necesidad; Prabhu es coautor de *Frugal Innovation* (2015).
11. **Búsqueda en vivo en GitHub: "tinyml raspberry pi pico" (9 nov 2026)**
    https://github.com/search?q=tinyml+raspberry+pi+pico
    Afirma: 38 repositorios en total para esa consulta, entre ellos `raspberrypi/pico-tflmicro` (753 estrellas), `edgeimpulse/firmware-pi-rp2xxx` y `henriwoodcock/pico-wake-word` (64 estrellas). La búsqueda se hizo con el conector de GitHub.
12. **Arducam Pico4ML — Kit de desarrollo TinyML para RP2040**
    https://core-electronics.com.au/arducam-pico4ml-rp2040-tinyml-dev-kit.html
    Afirma: placa basada en RP2040 con IMU, módulo de cámara, micrófono y pantalla LCD; incluye tres modelos TFLite preentrenados del libro oficial de TinyML (detección de personas, varita mágica, detección de palabra de activación); todo abierto (código, diseño y esquemáticos).

## Secundarias (marcadas como tales)

13. **MicrocontrollerTips — "What is TinyML?"**
    https://www.microcontrollertips.com/what-is-tinyml/
    Afirma: TinyML es un término acuñado por Pete Warden, responsable de ingeniería de TensorFlow Lite en Google; los modelos TinyML miden unas decenas de kilobytes y los dispositivos trabajan por debajo de 1 mW en los casos extremos. Fuente divulgativa, no primaria.
14. **"From Tiny Machine Learning to Tiny Deep Learning: A Survey" (arXiv:2506.18927, 2025)**
    https://arxiv.org/html/2506.18927v2/
    Afirma: TinyML se define típicamente como inferencia en dispositivos por debajo de 1 mW, a menudo con solo 32 a 512 KB de SRAM y flash limitada, sin sistema operativo ni aceleradores de coma flotante. Revisión (survey), no medición propia.
15. **Flux — "Raspberry Pi Pico 2 vs Pico: Key Differences (2026)" (16 sep 2026)**
    https://www.Flux.ai/p/blog/whats-new-in-the-raspberry-pi-pico-2-a-showdown-with-the-original-raspberry-pi-pico
    Afirma: Pico 2 lanzado en agosto de 2024; precio de lanzamiento 5 USD frente a 4 USD del Pico original; Cortex-M33 con FPU y DSP. Comparativa divulgativa, no fuente oficial.
16. **ElectroMaker — "Gesture Recognition Using Raspberry Pi Pico And Edge Impulse"**
    https://www.electromaker.io/project/view/gesture-recognition-using-raspberry-pi-pico-and-edge-impulse
    Afirma: el compilador EON de Edge Impulse permite correr con 25–55 % menos memoria y hasta 35 % menos flash que TensorFlow Lite for Microcontrollers con la misma exactitud. Tutorial que cita documentación de Edge Impulse; cifra no verificada de forma independiente.

## Visto y no usado

- Tabla de la DeepWiki de `tensorflow-micropython-examples` (hello_world en RP2040: ~60 KB RAM, ~600 KB flash, <3 ms): marcada en la propia página como estimación basada en huellas típicas, no como medición. No se usa ningún número de ahí.
- Artículos de blogs sobre consumo del Pico que citan mediciones propias sin hoja de datos (p. ej. 18 mA activo a 133 MHz): no usados; los números de consumo del README son solo los de la hoja de datos oficial.
