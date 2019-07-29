# *Control de procesos*

### *Índice*
- [Introducción a LabVIEW](#introducción-a-labview).
- [Primeros pasos en LabVIEW](#primeros-pasos-en-labview).
- [Primer programa](#primer-programa).
- [Segundo programa](#segundo-programa).

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

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image1.PNG)

En esa pantalla podemos seleccionar varias opciones entre las cuales están la sección de archivos, herramientas y ayuda.
Para iniciar un nuevo programa damos clic en la opción **File** y enseguida **New VI** 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image2.png)

Cuando abre un nuevo proyecto emergen dos ventanas, la primera pantalla que aparece es el **Panel frontal** o ventana de diseño de la aplicación mientras que la que aparece en segundo plano es la ventana de **Diagrama de bloques**.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image3.png)

Muchas veces es conveniente organizar las dos ventanas de forma tal que se dividan la pantalla cada una en una mitad para que se facilite el desarrollo del programa. Para lograr dicha distribución LabVIEW dispone de la combinación Ctrl+T. Una vez que se realiza esta acción se obtiene la siguiente distribución:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image4n.PNG)

La ventana del Panel frontal proporciona menús de herramientas y todos los controles necesarios para la aplicación, la ventana de controles emerge dando clic derecho dentro de la ventana de Panel frontal y luce de esta forma.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image4.png)

La programación se realiza mediante la selección de controles funcionales en la ventana del Panel frontal, y al seleccionar se agrega un bloque correspondiente en la ventana de Diagrama de Bloques.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image5.PNG)

Además de los controles funcionales como generadores de señales, botones, pantallas y gráficos, también se proporcionan controles decorativos que solo afectan al panel frontal. Estos permiten que los controles similares se agrupen visualmente y que el Panel frontal se vea similar al equipo real o sea tan detallado como se desee.
El diagrama de bloques es donde las entradas y salidas de los diversos controles se conectan entre sí. El programa se puede ejecutar, abortar y pausar desde el Panel frontal o el Diagrama de bloques.

El diagrama de bloques también proporciona ayudas para la resolución de problemas. La bombilla destacará la ruta de ejecución a medida que se ejecuta el programa. LabVIEW también permite pasar a través o sobre el código y se pueden establecer puntos de parada / observación.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image6.PNG)

Ahora que conocemos los puntos más básicos de LabVIEW podemos comenzar a realizar un programa sencillo para entender mejor el funcionamiento y familiarizarse con LabVIEW.

### *Primer programa*
Para la primer práctica se va a realizar un programa que permita hacer una suma de dos números. Para empezar, abrimos LabVIEW y como vimos anteriormente damos clic en **File** y después en **New VI**.
Una vez que hemos creado el nuevo VI daremos clic derecho sobre la ventana de Panel frontal para que aparezca la ventana de controles.
Usted crea el panel frontal con controladores e indicadores, los cuales son las terminales interactivas de entrada y salida del VI, respectivamente. Los controles pueden ser perillas, botones, barras deslizantes y otros dispositivos de entrada. Los indicadores son gráficas, LEDs y otras pantallas. Los controles simulan dispositivos de entrada de instrumentos y suministran datos al diagrama de bloques del VI. Los indicadores simulan dispositivos de salida de instrumentos y muestran los datos que el diagrama de bloques adquiere o genera.
Para esta práctica podemos usar un control numérico, una perilla o una barra deslizante, ya que estos representan datos numéricos. Para seleccionar alguno basta con acercar el puntero del mouse en la opción que dice **Numeric** y se abrirá otra ventana con las opciones mencionadas y muchas otras más que después veremos. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image7.png)

Usted puede seleccionar la que más le guste, en este caso usaremos la barra deslizante (Horizontal Pointer Slide), damos clic a la opción elegida y después regresará al Panel frontal, note que la figura de la opción seleccionada aparecerá en líneas punteadas, usted la podrá mover libremente dentro del Panel frontal hasta que encuentre el lugar donde desee fijarla, para esto solo debe dar clic en el lugar donde quiera fijarla y la figura del control aparecerá. De igual manera al hacer esto aparecerá un bloque en la ventana de Diagrama de bloques que representa el control colocado en el Panel frontal.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image8.png)

Por default todos los controles aparecerán con un nombre preestablecido, si desea cambiar el nombre de la barra o del control que usted coloco solo debe dar doble clic en el nombre preestablecido (en este caso donde dice Slide) y colocar el nombre que usted desee, note que al cambiar el nombre en el Panel frontal también cambiara en la ventana de Diagrama de bloques.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image9.png)

Como se sumarán dos números necesitaremos colocar otra barra, esto lo hacemos de la misma forma que la anterior.
Ya que ambas barras están listas ahora necesitaremos un indicador para que nos muestre el resultado de la suma, para ello nuevamente vamos a la ventana de controles y después en Numeric seleccionamos la opción **Numeric Indicator**, la fijamos en el Panel frontal y le cambiamos el nombre. Si hasta ahora todo va bien deberá tener un resultado similar a este: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image10.png)

Los objetos en la ventana del panel frontal aparecen como terminales en el diagrama de bloques. Las terminales son puertos de entrada y salida que intercambian información entre el panel frontal y diagrama de bloques. Son análogos a parámetros y constantes en lenguajes de programación basados en texto. Los tipos de terminales incluyen terminales de control o indicador y terminales de nodo. Las terminales de control e indicador pertenecen a los controles e indicadores del panel frontal.  Los nodos son objetos en el diagrama de bloques que tienen entradas y/o salidas y realizan operaciones cuando el VI se ejecuta. Son análogos a instrucciones, operaciones, funciones y sub rutinas en lenguajes de programación basados en texto. Los nodos pueden ser funciones, subVIs, Express VIs o estructuras. Las estructuras son elementos de control de procesos, como Estructuras de Casos, Ciclos For o Ciclos While. 
Para poder realizar la practica necesitaremos usar un nodo que nos proporcione la opción de suma, para localizar este nodo daremos clic derecho en la ventana de Diagrama de bloques y se abrirá una nueva ventana llamada **Functions**. La paleta de Funciones contiene los VIs, funciones y constantes que usted utiliza para crear el diagrama de bloques. La paleta de Funciones está dividida en varias categorías; usted puede mostrar y esconder categorías para cumplir con sus necesidades.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image11.png)

Ya que ha aparecido la ventana acercamos el puntero del mouse a la opción que dice **Numeric**, se abrirá una nueva ventana con varias funciones, para este caso necesitamos la de suma que aparece en la paleta de funciones como **Add**.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image12.png)

Seleccionamos el nodo de suma y después solo la fijamos en la ventana de Diagrama de bloques, este nodo cuenta con dos entradas y una salida, las entras se conectarán con los bloques de control numérico y la salida se conectará al bloque de indicador numérico, el resultado debería quedar similar a este: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image13.PNG)

De esta forma el programa ya puede funcionar, para ejecutarlo tenemos dos opciones, una es dar clic en **Run** y la otra es dar clic en **Run Continuously**, si elegimos la primer opción el programa se ejecutará una sola vez y se detendrá, por el contrario al elegir la segunda opción el programa seguirá corriendo hasta que le demos clic al botón de paro **Abort Execution**, esto funciona tanto en la ventana del Panel frontal como en la de Diagrama de bloques. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image14.png)

Para facilitar la visualización de los números que deseemos sumar podemos agregar un display a las barras deslizantes, esto se logra dando clic derecho sobre la barra y en la primer opción **Visible Items** damos clic y luego en **Digital Display**. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image15a.png)

Al dar clic en el icono de correr continuamente el programa empieza a trabajar y podemos ver que funciona correctamente haciendo varias pruebas.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image15.png)

Por ultimo solo queda guardar el archivo, para esto damos clic en **File** y después en **Save As…**

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image16.png)

Aparecerá una ventana y le damos un nombre al archivo, solo damos clic en **OK** y listo, el primer programa ha concluido. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image17.PNG)

### *Segundo programa*
Para la segunda practica vamos a realizar un programa que nos muestre el índice de masa corporal de una persona.
Una medida de la obesidad se determina mediante el índice de masa corporal (IMC), que se calcula dividiendo los kilogramos de peso por el cuadrado de la estatura en metros (IMC = peso [kg]/ estatura [m2]). Usando la siguiente tabla nos apoyaremos para saber en qué estado se encuentra la persona que ingrese sus datos en el programa.

| Composición corporal| Índice de masa corporal (IMC)|
| ----- | ---- |
| Bajo de peso | Menos de 18.5 |
| Normal | 18.5 – 24.9|
| Sobrepeso | 25.0 – 29.9 |
| Obesidad | Más de 30.0 |

Para empezar, ejecutamos LabVIEW y abrimos un nuevo VI, al igual que en el programa anterior necesitaremos controles numéricos y un indicador numérico para mostrar el resultado, colocaremos tres controles numéricos y en esta práctica usaremos una barra deslizante como indicador, pero en esta ocasión será una vertical, podemos encontrarla con el nombre de ** Vertical Pointer Slide** (esta se encuentra en el mismo menú que la barra deslizante horizontal que usamos en la primer practica), recordemos que damos clic derecho en la ventana de Panel frontal para que aparezca la ventana de controles y después damos clic en **Numeric** dentro de este menú podemos encontrarla. 
Hasta ahora debería tener un resultado similar a este: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image18.png)

Ya que hemos llegado a este punto ahora cambiamos los nombres de cada control numérico y de la barra deslizante, esto para que sepamos exactamente en qué control ira cada dato para el cálculo del IMC, recordando la formula esta nos pide la estatura de la persona y su peso en Kilogramos, entonces a un control le cambiaremos el nombre a *Peso [Kg]*, la otra a *Altura [m]* y la última a *Altura [cm]*. A la barra deslízate le cambiamos el nombre a IMC ya que aquí se mostrará el resultado. Entonces hasta aquí el programa debería lucir similar a este:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image19.png)

Como los valores según la tabla anterior van de 0 a mas de 30 entonces cambiaremos los valores de la barra deslizante para que esta concuerde,le daremos un valor mínimo de 10 y máximo de 40 en este caso, para cambiar los valores es similar a cuando cambiamos los nombres de los controles, solo damos doble clic sobre el valor inferior y el valor superior y colocamos los valores que queremos.  Ahora para que podamos visualizar el valor exacto que genere el programa podemos colocar un display a la barra deslizante, damos clic derecho y en la primera opción del menú que aparece **Visible Items** damos clic y después en **Digital Display**

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image20.png)

Hasta ahora el programa debería verse de esta forma:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image21.PNG)

Seguimos trabajando en el Panel frontal, esta vez usaremos la opción de **Adornos**, esto para colocar líneas en los límites de cada estado de la masa corporal y poder visualizar dentro del Panel frontal en qué situación se encuentra cada persona que ingrese sus datos al programa. Damos clic derecho en el Panel frontal y después en el menú de controles acercamos el puntero a la opción **Decorations** para que despliegue un submenú y elegimos una de las opciones de línea.

Imagen 22

Ya que elegimos una opción de línea colocamos una en cada valor correspondiente a la tabla para separar cada estado del IMC, y después escribiremos en cada nivel el estado en que se encuentra, para escribir solo damos doble clic en el lugar donde queremos escribir dentro del Panel frontal y escribimos el estado según los valores que tenemos, debería quedar similar a esto: 

Imagen23

Por ultimo eliminaremos las flechas de incremento y decremento de los controles para que se vea más presentable nuestro programa, esto es opcional, pero de hacerlo solo damos clic derecho sobre un control, en el menú que aparece llamado **Visible Items** damos clic y después damos clic a la opción **Increment/Decrement** para quitarlo, lo mismo con todos los controles

Image24

El resultado debe ser similar a este: 

Image25

Ahora que la parte del Panel frontal esta lista pasamos a trabajar en el Diagrama de boques, hasta ahora debe lucir así la ventana: 










