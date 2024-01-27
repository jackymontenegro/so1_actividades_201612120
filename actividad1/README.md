# Actividad 1 - Investigación conceptos de SO

## Tipos de Kernel y sus diferencias

**Monolítico:** Este tipo de Kernel trabaja todo en conjunto o en un mismo lugar, es decir que comparte el mismo espacio de direcciones con los controladores y con las interrupciones del sistema, algunos sistemas operativos que maneja este tipo de Kernel es Linux y versiones anteriores de Windows: 95, 98 y Millennium Edition.

**Microkernel:** En este tipo de Kernel se enfoca en funciones principales como la gestión de la memoria y la comunicación entre procesos por ejemplo entre los procesos de interacción entre el sistema operativo y el hardware, como teclado, mouse etc.o bien procesos como la inicialización del sistema, las interrupciones.Las demás funciones como los controladores y el sistema de archivo se ejecutan como procesos fuera del kernel. algunos sistemas operativos que manejan este tipo de kernel es QNX  y MINIX.

**Híbrido:** Este tipo de Kernel utiliza la combinación de los dos tipos anteriores manejando ciertos procesos en el espacio del Kernel y otros fuera de él, algunos sistemas operativos que manejan este tipo de Kernel es Windows NT y MacOS


## User vs Kernel Mode

**User Mode:** Este tipo de Modo, se utiliza para los programas que se ejecutan con un nivel de privilegios limitado, es decir que estos programas no necesitan alguna funcionalidad del hardware, esto para darle seguridad al sistema para que el programa a instalar no interfiera con los otros programas del sistema, por ejemplo si necesitamos instalar un juego este se debe instalar en User Mode ya que solo puede acceder a los recuerdos que el sistema operativo le asigne, es decir el juego no sería capaz de de apagar la computadora.

**Kernel Mode:** Este tipo de modo se utiliza para aquellos programas que necesitan privilegios altos como para instalar algún controlador ya que este necesita por ejemplo enviar señales a una impresora para que inicie su funcionalidad.

## Interrupciones vs Traps

**Interrupciones:** Una interrupción es una señal asíncrona que indica que algo externo o interno necesita atención del sistema operativo. Cuando se produce una interrupción el procesador suspende la ejecución actual y ejecuta una rutina para atender la interrupción, esto lo podemos ver cuando se presiona una tecla en el teclado, ya que se le envía una interrupción al sistema para indicar que se está presionando cierta tecla y que debe de escribirla o mostrarla en pantalla.

**Traps:** También se les conoce como excepciones, es una señal síncrona generada por el procesador en respuesta a ciertas condiciones durante una ejecución. Cuando se recibe una trap el procesador suspende la ejecución actual y ejecuta la rutina de manejo de la trampa. Por ejemplo cuando se intenta dividir en 0 el procesador detecta el error y genera un trap.