# Robotica-entradas-salidas
Desarrollado por Theylor Andres Amaya Villabon y  Juan Pablo Ortiz Mendoza


En el presente repositorio, se encuentra el desarrollo del laboratorio 2 de robótica enfocado en la gestión de entradas y salidas para el robot ABB IBR 140. Este trabajo se centra en la programación avanzada en el lenguaje RAPID y la utilización del módulo de entradas y salidas digitales integrado en el controlador IRC5.

Para llevar a cabo esta práctica, se establecen ciertos requisitos previos, incluyendo la instalación y activación de Robot Studio versión 5 o superior, la disponibilidad de las hojas de datos del manipulador industrial IRB 140 y del módulo 3HAC025917-001/00 DSQC 652, así como la presencia de manipuladores industriales ABB IRB 140.

El objetivo principal de esta práctica es abordar dos temas clave:

Programación intermedia en RAPID: Se explorará el manejo de bucles y condicionales en el lenguaje de programación RAPID.

Manejo del módulo de Entradas y Salidas digitales: Se abordarán las comunicaciones a través de señales digitales, proporcionando una comprensión más profunda de este componente fundamental en el control de robots industriales.

El trabajo a desarrollar en esta práctica implica la recepción de dos señales digitales de entrada y el control de dos salidas digitales. Durante el proceso, se llevará a cabo una revisión exhaustiva del funcionamiento de las señales digitales de entrada y salida en colaboración con el docente en el laboratorio. Además, se procederá a caracterizar y, si es necesario, ajustar los paneles de mando.

En el aspecto de programación, se crearán dos entradas y dos salidas digitales, configurándolas adecuadamente en el código de RAPID. La primera señal de entrada desencadenará una rutina de escritura sobre cualquier superficie y activará una luz indicadora. Al finalizar la rutina, el brazo del robot deberá regresar a su posición de "HOME", donde todos los ángulos articulares se establecerán en 0 grados.

# Solución planteada

En el siguiente video, presentamos la solución diseñada para este desafío, en la cual empleamos dos entradas digitales para controlar de manera efectiva el robot. En situaciones en las que el robot pueda comenzar en una posición aleatoria, lo primero que realiza nuestra rutina programada es llevarlo a la posición de "home", estableciendo así un punto de referencia inicial. Luego, el robot aguarda la activación de una de las dos señales de entrada.

Cuando se recibe la primera señal de entrada, el robot ejecuta una rutina de movimiento especialmente diseñada para llevar a cabo un dibujo específico. Una vez que la rutina de dibujo se completa, el robot regresa de manera precisa a la posición de "home". Como se puede observar en el video, al activar esta primera entrada, también se enciende un LED como una salida digital, lo que proporciona una indicación visual adicional de la ejecución de la rutina.

Por otro lado, al recibir la segunda señal de entrada, el robot se desplaza hacia una posición óptima que facilita el cambio de herramienta o cualquier otro proceso necesario en esa ubicación. En este punto, el robot apaga la luz que se había encendido previamente, indicando así un cambio de estado. En esta posición, el robot permanece a la espera de una nueva activación de la señal de entrada 2 para luego regresar nuevamente a la posición de "home".

Este enfoque meticulosamente diseñado y programado demuestra la versatilidad y precisión del robot ABB IBR 140 en la gestión de entradas y salidas digitales, brindando una solución eficiente para una variedad de aplicaciones en el campo de la robótica industrial. El video a continuación ilustra de manera visual y efectiva todo el proceso descrito anteriormente.

https://github.com/Theyloramaya/Robotica-entradas-salidas/assets/144027596/34c959bb-97a8-45c0-b79b-f2873ff75400

Entradas Digitales
Como se mencionó previamente, el controlador del Robot ABB IBR 140 (IRC5) cuenta con dos entradas digitales esenciales para el funcionamiento de nuestra solución. La primera de estas entradas desencadena una rutina específica de dibujo, al mismo tiempo que activa un indicador luminoso (LED). Tras la finalización de la rutina, el robot regresa a su posición inicial. Por otro lado, la segunda entrada tiene la tarea de dirigir el robot a una posición óptima para llevar a cabo un cambio de herramienta, y luego lo guía nuevamente a la posición de "home".


Salidas Digitales
En cuanto a las salidas, el LED mencionado anteriormente representa una de las salidas digitales clave en nuestro sistema. Este LED se mantiene encendido cuando se activa la primera entrada y se apaga automáticamente cuando se acciona la segunda entrada.

Posición de "Home"
La posición de "home" en nuestro contexto es la ubicación predeterminada proporcionada por el fabricante del robot. Sin embargo, es importante destacar que esta posición puede incluir un ajuste de offset en la articulación 2, lo que garantiza una configuración precisa y eficiente para nuestras operaciones.

![image](https://github.com/Theyloramaya/Robotica-entradas-salidas/assets/144027596/08755ad3-dd26-43e3-9126-31733109e66a)

Ejecución de la Rutina
A continuación, presentamos una representación gráfica de la rutina de movimiento que el robot realiza en respuesta a las señales de entrada mencionadas anteriormente. Esta figura ilustra de manera visual cómo el robot se mueve desde la posición de "home" hasta la ejecución de la rutina de dibujo, y finalmente regresa a la posición de "home".

![WhatsApp Video 2023-09-30 at 7 09 54 PM](https://github.com/Theyloramaya/Robotica-entradas-salidas/assets/144027596/9ca42c24-f9a5-471b-86d8-282b243ec883)


Posición de Mantenimiento
Para brindar una descripción detallada de la posición de mantenimiento del robot, proporcionamos la siguiente imagen que ofrece una representación gráfica de esta posición específica. Esta posición es fundamental para cualquier tarea de mantenimiento, ajuste o servicio que pueda ser necesario llevar a cabo en el robot ABB IBR 140.



