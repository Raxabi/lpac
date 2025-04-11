# lpac, el gestor de paquetes para GNU/Linux

lpac (**l**inux **pac**kager) es un gestor de paquetes moderno y ligero, escrito en Go, enfocado en mantener un sistema GNU/Linux limpio y ordenado.

## Why?

> Desde mi punto de vista, por las siguientes razones (grandes y no tan grandes):

### Un sistema más limpio

  - La mayoría de los gestores de paquetes para sistemas tipo UNIX colocan todos los paquetes instalados y sus dependencias dentro de directorios como /usr/bin, /usr/lib o /usr/include, sin distinguirlos de los archivos propios del sistema. Esto convierte a estos directorios en lo que llamo “directorios sucios”, y termina dejando el sistema lleno de dependencias cuya razón de estar ahí desconoces.

  - Cuando quieres desinstalar un paquete, a menudo sus dependencias y archivos de configuración no se eliminan, a menos que se lo indiques expresamente al gestor de paquetes. lpac invierte este comportamiento y lo hace de forma predeterminada.

  - lpac te obliga a mantener una estructura clara y un seguimiento de los paquetes instalados y sus dependencias, aislando las dependencias si solo un paquete las utiliza.

### Un experimento

Como único desarrollador de este software por ahora, quiero entender cómo funciona un gestor de paquetes. Y la mejor forma de lograrlo es implementando uno desde cero.

### Practise my Go abilities

Soy relativamente nuevo en el lenguaje Go. Como creo que permite crear software potente y limpio, me parece una buena idea practicar con él.
