# *Control de procesos*

### *Índice*
- [Introducción a LabVIEW](#introducción-a-labview).
- [Primeros pasos en LabVIEW](#primeros-pasos-en-labview).
- [Primer programa](#primer-programa).
- [Segundo programa](#segundo-programa).
- [Instalación del software NI VISA y del toolkit LINX](#instalación-del-software-ni-visa-y-del-toolkit-linx).
- [Tercer programa](#tercer-programa).
- [Cuarto programa](#cuarto-programa).
- [Quinto programa](#quinto-programa).
- [Sexto programa](#sexto-programa).
- [Séptimo programa](#séptimo-programa).
- [Octavo programa](#octavo-programa).
- [Noveno programa](#noveno-programa).
- [Decimo programa](#decimo-programa).

## *Introducción a LabVIEW*                            
*[Volver al Índice](#índice).*

LabVIEW es la contracción de las palabras en inglés *"Laboratory Virtual Instrument Engineering Workbench"*, y este es un entorno de programación gráfica usado por ingenieros y cientificos para desarrollar mediciones sofisticadas, pruebas y sistemas de control. LabVIEW puede integrar una gran variedad de dispositivos de hardware.
En este curso utilizaremos el hardware de comunicación serial y el DAQ (Data Adquisition) configurando el hardware en el MAX (Mesurement & Automation Explorer). Usted puede descargar la versión de LabVIEW estudiantil para Windows o para MAC, por lo que no necesita comprar el software. LabVIEW es un software de desarrollo gráfico y flexible creado por National Instruments, una compañía que crea productos de hardware y software que le permiten a las computadoras a ayudar a ingenieros y científicos a tomar mediciones, controlar procesos, analizar y guardar datos. National Instruments fue fundado hace 39 años en Texas a partir de personas que laboraban en la Universidad de Texas. Científicos e ingenieros en investigación, desarrollo, producción, pruebas e industrias de servicio como los semiconductores, automotriz, aeroespacial, electrónica, química, comunicaciones y farmacéutica han usado y continúan usando LabVIEW para desarrollar su trabajo. Por ejemplo SpaceX utiliza LabVIEW para llevar los cohetes Falcon 9 al espacio.
### *Instrumentos Virtuales*
Los programas de LabVIEW son llamados *"Instrumentos virtuales"* o *"VI's"* (Virtual Instrument). LabVIEW es diferente de otros lenguajes de programación como Python o C, ya que LabVIEW utiliza un lenguaje de programación gráfica conocida como el lenguaje de programación G,
para crear programas basados en simbolos gráficos. Labview utiliza una terminología familiar para científicos e ingenieros por lo que
sus símbolos o íconos gráficos son facilmente identificables para inspección visual. Se puede aprender LabVIEW incluso si se tiene poca 
experiencia en la programación.
## *Primeros pasos en LabVIEW*
*[Volver al Índice](#índice).*

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

Si usted desea aprender más sobre el uso de las funciones y de los controles en LabVIEW le dejo un [Enlace](http://www.ni.com/getting-started/labview-basics/esa/) que lo enviará a la página de National Instruments en la cual podrá encontrar un manual técnico que lo introduce a los conceptos requeridos para desarrollar un sistema básico con LabVIEW.

Ahora que conocemos los puntos más básicos de LabVIEW podemos comenzar a realizar un programa sencillo para entender mejor el funcionamiento y familiarizarse con LabVIEW.

## *Primer programa*
*[Volver al Índice](#índice).*

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

Como vimos el programa ya funciona correctamente, sin embargo, podemos agregar un ciclo **While** en la ventana de Diagrama de bloques. Similar a un Ciclo Do o a un Ciclo Repeat-Until en lenguajes de programación basados en texto, un Ciclo While en LabVIEW ejecuta el código que contiene hasta que ocurre una condición.
El Ciclo While está ubicado en la paleta Structures. Seleccione el Ciclo While en la paleta y después use el cursor para arrastrar una selección rectangular alrededor de la sección del diagrama de bloques que desea repetir.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/while.png)

Cuando suelte el botón del mouse, un borde del Ciclo While encierra la sección que seleccionó.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/while2.PNG)

Ahora nuestro programa está condicionado y para detenerlo dentro del mismo programa podemos colocar un botón de **Stop**, este se encuentra dentro del menú de controles en el submenú **Boolean**

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/while3.png)

Seleccionamos el botón y lo acomodamos dentro del Panel frontal, ahora tenemos el programa de esta forma:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/while4.png)

Por ultimo solo hacemos la conexión del bloque que representa el Stop con el punto rojo que tiene al lado para que al presiónalo en el Panel frontal el programa se detenga. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/while5.PNG)

Ahora podemos correr el programa de la misma forma que el anterior pero esta vez al dar clic en el botón de Stop del Panel frontal nuestro programa se detendrá.


Por ultimo solo queda guardar el archivo, para esto damos clic en **File** y después en **Save As…**

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image16.png)

Aparecerá una ventana y le damos un nombre al archivo, solo damos clic en **OK** y listo, el primer programa ha concluido. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image17.PNG)

## *Segundo programa*
*[Volver al Índice](#índice).*

Para la segunda practica vamos a realizar un programa que nos muestre el índice de masa corporal de una persona.
Una medida de la obesidad se determina mediante el índice de masa corporal (IMC), que se calcula dividiendo los kilogramos de peso por el cuadrado de la estatura en metros (IMC = peso [kg]/ estatura [m2]). Usando la siguiente tabla nos apoyaremos para saber en qué estado se encuentra la persona que ingrese sus datos en el programa.

| Composición corporal| Índice de masa corporal (IMC)|
| ----- | ---- |
| Bajo de peso | Menos de 18.5 |
| Normal | 18.5 – 24.9|
| Sobrepeso | 25.0 – 29.9 |
| Obesidad | Más de 30.0 |

Para empezar, ejecutamos LabVIEW y abrimos un nuevo VI, al igual que en el programa anterior necesitaremos controles numéricos y un indicador numérico para mostrar el resultado, colocaremos tres controles numéricos y en esta práctica usaremos una barra deslizante como indicador, pero en esta ocasión será una vertical, podemos encontrarla con el nombre de **Vertical Pointer Slide** (esta se encuentra en el mismo menú que la barra deslizante horizontal que usamos en la primer practica), recordemos que damos clic derecho en la ventana de Panel frontal para que aparezca la ventana de controles y después damos clic en **Numeric** dentro de este menú podemos encontrarla. 
Hasta ahora debería tener un resultado similar a este: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image18.png)

Ya que hemos llegado a este punto ahora cambiamos los nombres de cada control numérico y de la barra deslizante, esto para que sepamos exactamente en qué control ira cada dato para el cálculo del IMC, recordando la formula esta nos pide la estatura de la persona y su peso en Kilogramos, entonces a un control le cambiaremos el nombre a *Peso [Kg]*, la otra a *Altura [m]* y la última a *Altura [cm]*. A la barra deslizante le cambiamos el nombre a IMC ya que aquí se mostrará el resultado. Entonces hasta aquí el programa debería lucir similar a este:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image19.png)

Como los valores según la tabla anterior van de 0 a mas de 30 entonces cambiaremos los valores de la barra deslizante para que esta concuerde,le daremos un valor mínimo de 10 y máximo de 40 en este caso, para cambiar los valores es similar a cuando cambiamos los nombres de los controles, solo damos doble clic sobre el valor inferior y el valor superior y colocamos los valores que queremos.  Ahora para que podamos visualizar el valor exacto que genere el programa podemos colocar un display a la barra deslizante, damos clic derecho y en la primera opción del menú que aparece **Visible Items** damos clic y después en **Digital Display**

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image20.png)

Hasta ahora el programa debería verse de esta forma:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image21.PNG)

Seguimos trabajando en el Panel frontal, esta vez usaremos la opción de **Adornos**, esto para colocar líneas en los límites de cada estado de la masa corporal y poder visualizar dentro del Panel frontal en qué situación se encuentra cada persona que ingrese sus datos al programa. Damos clic derecho en el Panel frontal y después en el menú de controles acercamos el puntero a la opción **Decorations** para que despliegue un submenú y elegimos una de las opciones de línea.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image22.png)

Ya que elegimos una opción de línea colocamos una en cada valor correspondiente a la tabla para separar cada estado del IMC, y después escribiremos en cada nivel el estado en que se encuentra, para escribir solo damos doble clic en el lugar donde queremos escribir dentro del Panel frontal y escribimos el estado según los valores que tenemos, debería quedar similar a esto: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image23.PNG)

Por ultimo eliminaremos las flechas de incremento y decremento de los controles para que se vea más presentable nuestro programa, esto es opcional, pero de hacerlo solo damos clic derecho sobre un control, en el menú que aparece llamado **Visible Items** damos clic y después damos clic a la opción **Increment/Decrement** para quitarlo, lo mismo con todos los controles

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image24.png)

El resultado debe ser similar a este: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image25.PNG)

Ahora que la parte del Panel frontal esta lista pasamos a trabajar en el Diagrama de boques, hasta donde nos quedamos la ventana lucía así:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image26.PNG)

Ahora colocamos un While y analizamos la ecuación para hacer las conexiones adecuadas. Primero sabemos que hay que dividir los kilogramos entre la altura, por lo tanto, necesitaremos un nodo de división, después la altura sabemos que debe ir al cuadrado, entonces necesitaremos un nodo que nos permita elevar al cuadrado la altura, pero al tener dos bloques de altura (uno que cuenta los metros y el otro los centímetros) necesitamos un nodo que nos permita sumar los dos valores, entonces ahora sabemos los nodos que necesitamos para realizar las conexiones. Para encontrar estos nodos damos clic derecho en la ventana de Diagrama de bloques y después en la ventana que emerge llamada Functions damos clic en Numeric, dentro de este menú se encuentran todos los nodos que necesitamos. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image27.png)

Colocamos los nodos dentro del ciclo While y ahora el diagrama de bloques debe lucir algo así:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image28.PNG)

Hay que tener cuidado con la parte de la suma de la altura ya que si hacemos la suma directa tendremos un error en el resultado, esto es porque los centímetros los tomaría como si de metros se trataran, para evitar este error debemos dividir la cantidad que se coloque en centímetros entre 100 para tener un valor de altura correcto, si por ejemplo alguien que mida 1.70m ingresa sus datos el programa tomaría la información como si fueran 170m dando un grave error como resultado, para ello es la división, de esta forma el resultado será el correcto. Para poder dividir colocaremos una constante, esto lo hacemos entrando a la paleta de funciones después en Numeric y dentro de este se encuentra la opción llamada **DBL Numeric Constant**

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image29.png)

La seleccionamos y a esta le damos el valor de 100, ahora solo queda realizar las conexiones, como sabemos el peso debe dividir a la altura por lo tanto conectamos la salida de peso a la entrada de división, pasando a la altura realizamos la conexión de la suma de metros con centímetros, para ello conectamos las salidas de ambos bloques a las entradas del nodo de suma, según la ecuación la altura debe de elevarse al cuadrado, por lo tanto la salida del nodo de suma se conectara a la entrada del nodo de cuadrado y este último arrojara el valor final de la altura, entonces conectamos la salida del nodo de cuadrado a la entrada del nodo de división. El resultado de las conexiones debe quedar así:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image30.PNG)

Por ultimo solo queda conectar la salida del nodo de división al bloque de la barra deslizante, aquí podemos notar que este bloque solo cuenta con una salida pero no con una entrada, esto lo arreglamos dando clic derecho sobre el bloque y en el menú que despliega le damos clic a la opción **Change to Indicator**, haciendo pasa a ser un indicador y por lo tanto cambiara la salida que tenía por una entrada.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image31.png)

Ahora solo conectamos la salida del nodo que queda a la entrada del bloque y está casi listo, para terminar este ejercicio debemos colocar un botón de paro, esto lo podemos hacer dando clic derecho sobre el punto rojo que está en la parte inferior derecha, después damos clic en la opción **Create Control**, y aparecerá un nuevo bloque, de igual forma aparecerá uno en el Panel frontal y este servirá para detener el programa. 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image32.png)

En el Panel frontal acomodamos el nuevo control donde mejor nos parezca y ya solo queda probar el programa, lo corremos e ingresamos nuestros datos.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image33.PNG)

Puede corroborar el resultado en internet para que vea que el programa funciona correctamente.

## *Instalación del software NI VISA y del toolkit LINX*
*[Volver al Índice](#índice).*

Para las siguientes practicas se utilizará comunicación serial con **Arduino**, por lo cual es necesario instalar el software controlador **NI-VISA** que proporciona la interfaz de programación entre el hardware (Arduino) y el entorno de desarrollo de aplicaciones LabVIEW, y el toolkit **LINX** de Digilent/LabVIEW MakerHub.**LINX**, es una herramienta de fuente abierta de Digilent y diseñada para facilitar el uso y desarrollo de aplicaciones embebidas usando LabVIEW. **LINX** incluye VI's ejemplares sobre los sensores embebidos más comunes, así como aplicaciones de programación de hardware agnóstico para tener acceso a periféricos como Entradas/Salidas digitales, Entradas/Salidas analógicas, PWM, I2C, SPI y UART. Ya sea que esté controlando por un hardware remoto como un chipKIT o Arduino por USB/Serial, Ethernet o Wi-Fi o implementando VI's para ejecutar en plataformas como Raspberry Pi 2/3, **LINX** y LabVIEW hacen más sencilla la visualización de los datos con los que está trabajando, depurando su código y creando aplicaciones embebidas avanzadas de manera rápida.
Para instalar todo lo necesario para las siguientes practicas siga los siguientes pasos:

### *Instalación del Software NI-VISA*

Una vez instalado el software LabVIEW se debe instalar el software controlador NI-VISA para permitir la comunicación con el sistema embebido Arduino, para esto se descarga de forma gratuita el software directamente de la página oficial de National Instruments a través de una cuenta personal creada por el usuario. La versión del software controlador depende de la versión del software LabVIEW que se esté utilizando, en el siguiente [enlace]( http://www.ni.com/es-mx/support/downloads/drivers/download.ni-visa.html#305862) podrá encontrar el que se adecue a su versión.

Descargue y ejecute el archivo autoextraíble. Para instalar NI-VISA y todos los archivos necesarios del controlador debe seguir los siguientes pasos:
1. Ejecutar el archivo autoextraíble.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image34.PNG)

2. Seleccionar la carpeta de destino de instalación en el disco local C.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image35.PNG)

3. Seleccionar la opción para recibir notificaciones software NI-VISA para facilitar actualizaciones (este paso es opcional si no desea recibir notificaciones sobre actualizaciones).

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image36.PNG)

4. A continuación, se visualizan todos los archivos que se instalaran en el controlador.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image37.PNG)

5. Se procede a aceptar el contrato de licencia.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image38.PNG)

6. Para que Windows no interrumpa el proceso de instalación, seleccionar el check-box correspondiente al acuerdo de confianza que hace referencia a la instalación de softwares provenientes de National Instruments Corporation.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image39.PNG)

7. Se procede a aceptar el proceso de instalación del software NI-VISA y sus controladores.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image40.PNG)

8. Una vez terminado el proceso de instalación se procede a reiniciar el equipo y listo, tendrá instalado NI-VISA en su equipo.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image41.PNG)

### *Instalación del toolkit LINX*

Para obtener este toolkit primero debemos ir al siguiente [enlace](http://sine.ni.com/nips/cds/view/p/lang/es/nid/212478) el cual nos dirigirá a la página de National Instruments, como se ve en la imagen damos clic en recursos y después en descargar.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image42.png)

Después le pedirán crear una cuenta o si ya tiene una ingresar para poder descargar, una vez que ha ingresado da clic en Download Toolkit, y después en Abrir VIPMHelper.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image43.png)

Se abrirá una ventana como esta: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image44.PNG)

A continuación, se procede a realizar la instalación del toolkit LINX, podemos cambiar la versión de LabVIEW que se muestra si es necesario y después damos clic en el botón Install

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image45.png)

Como siguiente paso, se procede aceptar los acuerdos de licencia del toolkit LINX de Digilent.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image46.PNG)

Una vez aceptados los acuerdos de licencia, automáticamente se inicia la instalación del toolkit LINX de Digilent. Para finalizar la instalación se procede a dar clic en el botón Finish.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image47.PNG)

Si todo salió bien ahora tenemos todo lo neceario para conectar LabVIEW con Arduino y empezar las siguientes practicas.

## *Tercer programa*
*[Volver al Índice](#índice).*

Ahora estamos listos para probar nuestra instalación de LabVIEW / LINX y comenzar a probar nuestra interfaz de LabVIEW para Arduino. Lo primero que debe hacer es ir a la ventana principal de LabVIEW; luego, haga clic en **Tools** y luego en **MakerHub**, que es el enlace para acceder a la interfaz LINX. Luego, haga clic en LINX y, finalmente, haga clic en **LINX Firmware Wizard**

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image48.png)

Esto lo llevará a la interfaz gráfica LINX que utilizaremos para configurar nuestra placa Arduino para la practica. Tenga en cuenta que este paso debe hacerse solo una vez; Una vez que el software correcto esté cargado en la placa Arduino, no tendrá que volver a tocarlo. 
El asistente comienza preguntándonos qué tipo de Arduino vamos a utilizar. Configure esta primera página seleccionando la opción que le convenga. En este caso estaré usando un Arduino mega por lo que la configuración queda así:

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image49.PNG)

Damos clic en Next y después de eso, se le pedirá que seleccione el puerto serie en el que desea que se comunique la interfaz. Como solo he conectado una placa Arduino en ese momento, solo se puede seleccionar el puerto que Windows llama COM8. Una forma muy simple de encontrar el puerto COM o serie que corresponde a su placa Arduino es ir al panel de control y después a dispositivos e impresoras, aquí aparecerá la tarjeta Arduino que este conectada y el puerto COM correspondiente. Una vez que se eligio el puerto damos clic en Next.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image50.png)

Nevamente damos next en la ventana que aparece.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image51.PNG)

Finalmente damos clic en Launch Example que es para cargar un programa de ejemplo y comenzará a cargar el firmware en la placa Arduino.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image52.PNG)

Al terminar de cargar el programa se abrira un nuevo VI igual a este: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image53.PNG)

Como puede ver, este VI es realmente simple, ya que puede controlar el valor de un pin digital del Arduino haciendo clic en el botón verde en el lado derecho. Hay dos cosas que debe modificar aquí antes de poder iniciar el VI. Primero, debe configurar el puerto serie correcto en el cuadro **Serial Port**. Simplemente elija el nombre de su puerto, y se completará automáticamente lo que está escribiendo. Luego, debe establecer qué pin desea controlar. Simplemente puede usar el pin número 13 aquí, ya que está conectado al LED incorporado en la placa Arduino. Si elige cualquier otro pin, podrá construir un circuito simple en su placa, como se muestra en la ilustración en el lado izquierdo del VI.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image54.png)

Ahora correremos el VI, para hacerlo simplemente haga clic en la flecha pequeña en la barra de herramientas, entonces espere un momento, el VI ahora intentará inicializar la comunicación con el Arduino. Si hace clic en algo de inmediato, puede producir un error. usted sabrá que el proceso de inicialización se completa cuando los LED's de puerto de la placa Arduino (TX y RX) están encendidos. Ya que el programa esta completamente listo podemos ponerlo a prueba, en el Panel frontal podemos ver que el boton verde se encuentra apagado.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image55.PNG)

De la misma forma que en Panel frontal el led **L** de la placa Arduino se encuentra apagado.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/arduinoap.png)

Si presionamos el boton del Panel frontal este se encendera.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image552.PNG)

De la misma forma el led **L** de la placa Arduino se enciende al mismo tiempo que presionamos el boton verde.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/arduinoen.png)

Verá que el LED de la placa Arduino se enciende o apaga al mismo tiempo que presiona el boton del Panel frontal, ahora hemos conectado exitosamente la placa Arduino con LabVIEW.

Para ver los detalles vaya a la ventana de Diagrama de bloques y aparecerá algo como esto: 

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/image56.PNG)

Ahora analicemos como es que funciona este primer programa para poder entender los siguientes.
Tenemos cuatro bloques que podríamos decir que son los principales, estos son: 
### 1.Open Serial
Abre una conexión en serie a un dispositivo LINX remoto.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/openlinx.PNG)
 
Como entradas tenemos:

**Serial Port**

Especifica el puerto COM del dispositivo LINX remoto.

**Baund Rate Override**

(Opcional) Cuando se especifica, permite al usuario anular la velocidad de transmisión predeterminada utilizada para la comunicación en serie. De forma predeterminada, LINX establece la comunicación utilizando una velocidad en baudios de 9600 y luego negocia la velocidad máxima en baudios del dispositivo LINX remoto y restablece la comunicación a esa velocidad máxima. Si se proporciona una entrada de anulación de velocidad en baudios, se utilizará la velocidad en baudios máxima. Esto es útil cuando se usan abstracciones UART que no pueden cambiar las velocidades en baudios sobre la marcha (Xbee, por ejemplo).

**Error In** 

Describe las condiciones de error que ocurren antes de que se ejecute este nodo. Esta entrada proporciona la funcionalidad de error estándar.

Como salidas tenemos:

**LINX Resource** 

Contiene recursos de conexión LINX.

**Device Name**

El nombre del dispositivo LINX remoto.

**Error Out** 

Contiene información de error. Esta salida proporciona la funcionalidad de error estándar.

### 2.Digital Write 1 Chan
Escribe un valor en el canal de salida digital especificado.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/dwritelinx.PNG)
 
Como entradas tenemos:

**LINX Resource**

Contiene recursos de conexión LINX.

**DO Channel** 

Especifica el canal de salida digital para escribir.

**Output Value**

Especifica el valor digital para escribir.

**Error In**

Describe las condiciones de error que ocurren antes de que se ejecute este nodo. Esta entrada proporciona la funcionalidad de error estándar.

Como salidas tenemos:

**LINX Resource**

Contiene recursos de conexión LINX.

**Error Out** 

Contiene información de error. Esta salida proporciona la funcionalidad de error estándar.

### 3.Close

Cierre la conexión al dispositivo LINX remoto y libere cualquier recurso de E / S local.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/closelinx.PNG)
 
Como entradas tenemos:

**LINX Resource**

Contiene recursos de conexión LINX.

**Error In** 

Describe las condiciones de error que ocurren antes de que se ejecute este nodo. Esta entrada proporciona la funcionalidad de error estándar.

Como salidas tenemos:

**Error Out** 

Contiene información de error. Esta salida proporciona la funcionalidad de error estándar.

### 4.Simple Error Handler.
Indica si se produjo un error. Si se produjo un error, este VI devuelve una descripción del error y, opcionalmente, muestra un cuadro de diálogo.
Este VI llama al General Error Handler VI y tiene la misma funcionalidad básica que el General Error Handler pero con menos opciones.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/Simpleerror.png)
 
En este bloque normalmente usaremos solamente la entrada llamada Error In, sin embargo, se explicarán todas las entrada y salidas del bloque.

**Error Code**

Es un código de error numérico. Si el **Error In** indica un error, el VI ignora el **Error Code**. Si no, el VI lo prueba. Un valor distinto de cero significa un error.

**Error Source**

Es una cadena opcional que puede usar para describir la fuente del **Error Code**.

**Type of Dialog**

Determina qué tipo de cuadro de diálogo mostrar, si lo hay. Independientemente de su valor, el VI emite la información de error y el mensaje que describe el error.

![LabVIEW image](https://github.com/FelixGil55/Control-de-Procesos/blob/master/Curso%20LabVIEW%20im%C3%A1genes/cuadrolinx.png)

**Error In**

Describe las condiciones de error que ocurren antes de que se ejecute este nodo. Esta entrada contiene estado, código y fuente, que proporcionan la funcionalidad de un error estándar del elemento del clúster. 

**Error?**

Devuelve VERDADERO si se produce un error. Si este VI encuentra un error, establece los parámetros en el clúster de error.

**Code Out**

Es el código de error indicado por un **Error In** o un **Error Code**.

**Source Out** 

Indica la fuente del error.

**Error Out** 

Contiene información de error. Esta salida proporciona la funcionalidad de error estándar.

**Message**

Describe el código de error que ocurrió, la fuente del error y una descripción del error. Si el VI no devuelve una descripción del error, usted puede realizar varias acciones para encontrar la descripción del código de error. Si existe más de una descripción para el mismo código de error, el VI muestra todas las descripciones, separadas por un Or.

## *Cuarto programa*
*[Volver al Índice](#índice).*

few



## *Quinto programa*
*[Volver al Índice](#índice).*

En esta práctica controlaremos un motor de DC que esté conectado a la placa Arduino. Se va a controlar la dirección y la velocidad directamente desde Interfaz gráfica de LabVIEW.
Para el motor, se eligió un pequeño motor de 5V DC. Puede elegir cualquier marca que desee para el motor lo importante es que tiene que funcionar a 5V para que pueda alimentarse directamente desde Arduino. También puede conseguir un motor que use voltajes o corrientes más altas, pero deberá modificar la configuración de hardware ligeramente.
También necesitará el controlador de motor L293D para controlar el motor desde Arduino. Este es un chip dedicado que usaremos para controlar fácilmente el motor desde LabVIEW. Usted también puede usar una alternativa a este chip; por ejemplo, puede usar un Arduino shield que ya integra chips similares en el tablero. Este es, por ejemplo, el caso del Arduino motor shield, que integra el chip L298D. Sin embargo, necesitaria modificar ligeramente el código si está utilizando un shield en lugar del chip solo.
Finalmente, necesitará una placa de pruebas y jumpers para hacer todas las conexiones.

#### Configuración de hardware
Veamos ahora cómo ensamblar los diferentes componentes del proyecto. Este esquema lo ayudará a visualizar las conexiones entre los diferentes componentes:

Motor1

Para ensamblar los componentes, siga los siguientes pasos:

1. Primero, coloque el chip L293D en el centro de la placa de pruebas.

2. Luego, cuide la fuente de alimentación; conecte el pin superior izquierdo y el pin inferior derecho del chip L293D al pin Arduino 5V.

3. Luego, conecte uno de los pines en el centro inferior del chip al Pin Arduino GND.

4. Después de eso, conecte las señales de comando provenientes del Arduino, que estará en los pines 4, 5 y 6, y la placa Arduino Uno.

5. Finalmente, conecte el motor de DC al chip L293D, como se muestra en el esquema.

Para ayudarlo, aquí hay un [enlace](http://users.ece.utexas.edu/~valvano/Datasheets/L293d.pdf) a la configuración de los pines del chip L293D.

Así es como debería verse al final:

Motor2

Cuando haya terminado, puede pasar al siguiente paso, construir el VI en LabVIEW para controlar el motor DC.

#### Escribiendo el programa LabVIEW
Para comenzar el proceso, abra LabVIEW y cree un nuevo VI en blanco. Lo primero que colocaremos en el VI en blanco es un bucle While. Este bucle es requerido para cualquier placa Arduino que desee controlar a través de LINX, y todos los Arduino Los comandos deberán colocarse dentro de este bucle.
Después de eso, colocaremos nuestros primeros elementos del paquete LINX. Los primeros elementos que necesitamos colocar son los elementos de inicialización y detención de LINX, que son necesarios para decirle al software dónde comenzar y dónde parar. Puede encontrar ambas cajas en el panel de funciones yendo al submenú Makerhub.

Desde el mismo submenú, coloque dos bloques de Digita Write (que se utilizarán para controlar la dirección del motor) y un bloque PWM (que se utilizará para controlar la velocidad del motor). Tenga en cuenta que puede encontrar estos bloques en el menú Periféricos. Este es el resultado:

Motor3

Necesitamos un bloque PWM aquí para controlar la velocidad del motor. PWM significa Modulación de ancho de pulso y se utiliza para controlar la velocidad del motor o para atenuar los LED, por ejemplo. En la placa Arduino, es una salida de la placa que se puede configurar de 0 a 255 en algunos pines de la placa Uno.
Ahora, necesitamos alguna forma de decirle a LabVIEW en qué orden queremos que el sketch sea ejecutado. Aquí es donde entran en juego el error y el LINX resource. Simplemente comienza desde el bloque de inicialización en el lado izquierdo y encuentre el pin de error en el bloque.
Luego, conecte el pin de salida de error de este bloque al pin de entrada de error del primer bloque digital y así sucesivamente hasta el bloque final. Después de eso, haga lo mismo con los pines del LINX resource. También agregue un controlador de errores simple al final del VI, justo después de la parada bloquear. Este controlador se puede encontrar en el menú Diálogo e interfaz de usuario.

Motor4

Ahora que tenemos la parte principal de nuestro proyecto, alimentaremos los bloques con algunas entradas, primero agregue un puerto serie al bloque de inicialización yendo al pin del puerto serie del bloque y haciendo clic derecho sobre él. Luego, vaya a Create y luego a Control, para agregar automáticamente una entrada de puerto serie. Notara que el control correspondiente también se agrega automáticamente al Panel frontal. Cambie el nombre de este control a Puerto serie para que podamos identificarlo en el Panel frontal. También crearemos el mismo tipo de controles para los pines de los bloques que colocamos anteriormente. Para cada bloque, simplemente agregue entradas haciendo clic derecho en la entrada del pin y luego yendo a Create y después a Control. Además, cambie el nombre de todos estos controles para que sepamos lo que significan más adelante en el Panel frontal.

Motor5

También necesitamos agregar una condición final para el bucle While. Para hacerlo, necesitamos conectar el pequeño círculo rojo que se encuentra en la esquina inferior derecha al While Loop. Simplemente conectaremos el cable de error directamente a este círculo rojo. Para hacerlo, solo seleccione el pin de entrada del círculo rojo y conéctelo al error inferior cable dentro del VI.

Motor6

Ahora alimentaremos los valores de los diferentes bloques que cambiaremos desde el Panel frontal para controlar el motor. En esta etapa, lo mantendremos simple: tendremos algunos controles de encendido / apagado para la dirección y un cuadro de texto simple para la velocidad del motor.
Primero, establezcamos la dirección que necesitamos para alimentar los dos primeros bloques LINX en nuestro VI. El chip L293D requiere ser alimentado con señales opuestas en los dos pines de dirección para que el motor gire en una dirección dada. Por ejemplo, cuando el primer Digital Write está activado, queremos que el segundo esté desactivado y viceversa.
Para hacerlo, crearemos un bloque de control en el primer bloque de escritura digital, nuevamente haga clic derecho en el pin de entrada y luego vaya a Create/Control. Entonces iremos al menú Funciones, en Booleanos, elija un elemento Not y úselo para conectar nuestro control al segundo canal de escritura digital. De esta manera, estamos seguros de que estos dos siempre estará en estados opuestos.
Finalmente, también haga lo mismo para el bloque PWM creando un control para el valor del PWM. Este simplemente se mostrará como una entrada de texto dentro del Panel frontal. Lo haremos también que cambie el nombre de este pin como Velocidad del motor para que sepamos lo que significa en el Panel frontal.

Motor7

Ahora puede volver al Panel frontal y ver todos los elementos que estaban agregado automáticamente para usted. Organícelos un poco para que sea más fácil de controlar el motor.

Motor8

Es hora de probar el VI. Primero, configure todos los pines correctos y su puerto serie, como se muestra en la imagen anterior. Luego, haga clic en la pequeña flecha en la barra de herramientas para comenzar el VI.
Ahora puede ingresar un valor entre 0 y 255 en la entrada Velocidad del motor; ya verás que el motor comienza a girar de inmediato. Tenga en cuenta que tenemos que usar un valor entre 0 y 255, ya que el valor de salida PWM de Arduino Uno está codificado en 8 bits, por lo que tiene 256 valores. También puede usar el botón verde para cambiar la dirección del motor.

#### Actualizando la interfaz
Ahora tenemos un control básico para nuestro motor DC, pero podemos hacerlo mejor. De hecho, no es tan conveniente escribir la velocidad del motor en el panel frontal cada vez que desee para modificar algo es por eso que presentaremos otro tipo de control llamado Mando de control.
Para agregar dicho control, comience desde el Panel frontal y haga clic derecho para abrir los Controles panel. Luego, vaya a Numérico y seleccione el control Knob del menú.

Motor9

Ahora, la perilla está insertada en el Panel frontal, puede volver al diagrama de bloques donde puede eliminar el control de texto anterior del bloque PWM y conectar el nuevo en lugar. También puede cambiarle el nombre a Velocidad del motor.

Motor10

Ahora, también tenemos que configurar la perilla para que su valor de salida coincida con el aceptado del bloque PWM. Recuerde que el bloque PWM de LINX acepta valores entre 0 y 255.
Para hacerlo, simplemente haga clic derecho en el bloque Knob y haga clic en Propiedades. En este menú haga clic en Scale y cambie los valores mínimo y máximo, como se muestra en la siguiente captura de pantalla:

Motor11

Ahora puede volver al Panel frontal. Verá que la perilla ahora muestra los valores correctos, que van de 0 a 255. También puede cambiar el tamaño de la perilla en este punto para qué sea más fácil de usar.

Motor12

Ahora es el momento de probar la interfaz modificada. Como hizo antes, haga clic en la pequeña flecha dentro de la barra de herramientas. Ahora puede simplemente girar la perilla para cambiar instantáneamente la velocidad de rotación del motor.

## *Sexto programa*
*[Volver al Índice](#índice).*






## *Séptimo programa*
*[Volver al Índice](#índice).*







## *Octavo programa*
*[Volver al Índice](#índice).*






## *Noveno programa*
*[Volver al Índice](#índice).*







## *Decimo programa*
*[Volver al Índice](#índice).*







