# *Control de procesos*
## *Introducción a LabVIEW*
LabVIEW es la contracción de las palabras en inglés *"Laboratory Virtual Instrument Engineering Workbench"*, y este es un entorno de programación gráfica usado por ingenieros y cientificos para desarrollar mediciones sofisticadas, pruebas y sistemas de control. LabVIEW puede integrar una gran variedad de dispositivos de hardware.
En este curso utilizaremos el hardware de comunicación serial y el DAQ (Data Adquisition) configurando el hardware en el MAX (Mesurement & Automation Explorer). Usted puede descargar la versión de LabVIEW estudiantil para Windows o para MAC, por lo que no necesita comprar el software. LabVIEW es un software de desarrollo gráfico y flexible creado por National Instruments, una compañía que crea productos de hardware y software que le permiten a las computadoras a ayudar a ingenieros y científicos a tomar mediciones, controlar procesos, analizar y guardar datos. National Instruments fue fundado hace 39 años en Texas a partir de personas que laboraban en la Universidad de Texas. Científicos e ingenieros en investigación, desarrollo, producción, pruebas e industrias de servicio como los semiconductores, automotriz, aeroespacial, electrónica, química, comunicaciones y farmacéutica han usado y continúan usando LabVIEW para desarrollar su trabajo. Por ejemplo SpaceX utiliza LabVIEW para llevar los cohetes Falcon 9 al espacio.
### *Instrumentos Virtuales*
Los programas de LabVIEW son llamados *"Instrumentos virtuales"* o *"VI's"* (Virtual Instrument). LabVIEW es diferente de otros lenguajes de programación como Python o C, ya que LabVIEW utiliza un lenguaje de programación gráfica conocida como el lenguaje de programación G,
para crear programas basados en simbolos gráficos. Labview utiliza una terminología familiar para científicos e ingenieros por lo que
sus símbolos o íconos gráficos son facilmente identificables para inspección visual. Se puede aprender LabVIEW incluso si se tiene poca 
experiencia en la programación.
## *Primeros pasos en LabVIEW*
Después de la breve introducción ahora empezaremos a trabajar con el software, para este curso se usará LabVIEW 2017.
Primero se ejecuta el programa y se abrirá una ventana similar a la siguiente:

![GitHub Logo](image1.PNG)

En esa pantalla podemos seleccionar varias opciones entre las cuales están la sección de archivos, herramientas y ayuda.
Para iniciar un nuevo programa damos click en la opción **File** y enseguida **New VI** 

![GitHub Logo](image2.png)

Cuando abre un nuevo proyecto se abren dos ventanas, la primera pantalla que aparece es el **Panel frontal** o ventana de diseño de la aplicación mientras que la que aparece en segundo plano es la ventana de **Diagrama de bloques**.

![GitHub Logo](image3.png)

Muchas veces es conveniente organizar las dos ventanas de forma tal que se dividan la pantalla cada una en una mitad para que se facilite el desarrollo del programa. Para lograr dicha distribución LabVIEW dispone de la combinación Ctrl+T. Una vez que se realiza esta acción se obtiene la siguiente distribución:

![GitHub Logo](image4n.png)

La ventana del Panel frontal proporciona menús de herramientas y todos los controles necesarios para la aplicación, la ventana de controles emerge dando click derecho dentro de la ventana de Panel frontal y luce de esta forma.

![GitHub Logo](image4.png)

La programación se realiza mediante la selección de controles funcionales en la ventana del Panel frontal, y al seleccionar se agrega un bloque correspondiente en la ventana de Diagrama de Bloques.

![GitHub Logo](image5.PNG)

Además de los controles funcionales como generadores de señales, botones, pantallas y gráficos, también se proporcionan controles decorativos que solo afectan al panel frontal. Estos permiten que los controles similares se agrupen visualmente y que el Panel frontal se vea similar al equipo real o sea tan detallado como se desee.
El diagrama de bloques es donde las entradas y salidas de los diversos controles se conectan entre sí. El programa se puede ejecutar, abortar y pausar desde el Panel frontal o el Diagrama de bloques.

El diagrama de bloques también proporciona ayudas para la resolución de problemas. La bombilla destacará la ruta de ejecución a medida que se ejecuta el programa. LabVIEW también permite pasar a través o sobre el código y se pueden establecer puntos de parada / observación.

![GitHub Logo](image6.PNG)

Ahora que conocemos los puntos más básicos de LabVIEW podemos comenzar a realizar un programa sencillo para entender mejor el funcionamiento y familiarizarse con LabVIEW.

### *Primer programa*


