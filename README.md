## UNIVERSIDAD DE LAS FUERZAS ARMADAS ESPE
![](https://github.com/erickfi/Practica-5/blob/master/Img/Escudo.jpg)
### Práctica de laboratorio N° 8
## AMPLIFICADOR OPERACIONAL
**Autores:** Figueroa Erick, León Jipshon,Viracucha William.
### 1. PLANTEAMIENTO DEL PROBLEMA

Cuando se considera al amplificador operacional como un elemento ideal, sus características son:
- Impedancia de entrada infinita.
- Impedancia de salida nula.
- Ganancia de tensión infinita
- Ancho de banda infinito.
- Salida nula.
- cuando ambas entradas son iguales, corriente nula de polarización a fin de generar una respuesta funcional en sus entradas.
- voltaje nulo de desviación u offset (lo que implica una perfecta adaptación entre las etapas de entrada), y ausencia de desviación en sus características con los cambios de temperatura y valores de voltaje aplicados.

Sin embargo, en la realidad, el amplificador operacional presenta desviaciones con respecto a este comportamiento ideal, algunas de las cuales son las siguientes:
> 1. Voltaje de desviación (offset) a la entrada (Voff): en un op amp ideal, cuando se cortocircuitan las entradas, la salida se anula. En un amplificador operacional real,
para que la salida se anule, es necesario aplicar una pequeña tensión (Voff) entre las entradas. Este voltaje se origina en el desequilibrio entre las dos etapas de
entrada y varía con los cambios de temperatura, envejecimiento y, en menor medida, con los valores de los voltajes de polarización y de entrada.

> 2. Corriente de desviación (Ioff): debido al desequilibrio interno de los puertos de entrada, las corrientes DC absorbidas por los terminales N y P no son exactamente iguales. La diferencia entre ambas es la corriente de desviación. 

> 3. Impedancia de entrada (Zin): en un op amp real, la impedancia de entrada es grande, pero no infinita. Además, es fuertemente dependiente de la frecuencia, ya que incorpora un elemento capacitivo, lo cual hace que disminuya con la frecuencia. No obstante, a bajas frecuencias, puede considerarse que la impedancia de entrada es resistiva pura (Rin).

> 4. Impedancia de salida (Zout): la impedancia de salida de un op amp es pequeña, pero diferente de cero. Típicamente, se ubica en el rango de las decenas a centenas de ohmios. Nuevamente, a bajas frecuencias puede considerarse que esta impedancia es resistiva pura (Ro).

> 5. Ganancia de lazo abierto (A): en este caso, los amplificadores operacionales comerciales se aproximan mucho al caso ideal, ya que para este parámetro se consiguen valores de 250 000 y más. Disminuye con la frecuencia. 

### 2. OBJETIVOS
#### Objetivo General

- Simular de manera eficaz un amplificador operacional, reconociendo su funcionamiento, aplicaciones y gráficas.

#### Objetivos Específicos
- Verificar el principio de funcionamiento de un amplificador operacional.
- Analizar algunas aplicaciones básicas con el amplificador operacional.
- Familiarizarse con el uso de instrumentos de medida.

### 3. MARCO TEÓRICO
Un amplificador operacional (abreviadamente, op amp, del inglés operational amplifier) es un amplificador electrónico de voltaje con muy alta ganancia, entradas diferenciales y, generalmente, una única salida. Según Sadiku (2006)

> El amplificador operacional es una unidad electrónica que se comporta como una fuente de tensión controlada por tensión, es un elemento de circuitos activo diseñado para realizar operaciones matemáticas de suma, resta, multiplicación, división, diferenciación e integración.

En otras palabras y dentro de los contextos estudiados, un operador operacional es un circuito integrado, que consta de un complejo sistema de resistores, transistores, capacitores y diodos. Existen diversos tipos de amplificadores, uno habitual es el empaque en línea doble (dual in-line package, DIP por sus siglas en inglés) de ocho terminales. A continuación se presenta el circuito integrado así como su símbolo dentro de un diagrama.

![](https://github.com/erickfi/practica-8/blob/master/Imgs/amplificador%20operacional.PNG)

- La terminal 8 no se usa.
- Las terminales 1 y 5 por lo general no se conectan a componentes externos y suelen conectarse entre ellas como señal de salida.
- La entrada inversora, terminal 2.
- La entrada no inversora, terminal 3.
- La salida, terminal 6.
- El suministro de potencia positivo V+, terminal 7.
- El suministro de potencia negativo V-, terminal 4.

Las entradas se han marcado con los signos menos (-) y más (+) para especificar las entradas inversora y no inversora, respectivamente. 
Una entrada aplicada a la terminal no inversora aparecerá con la misma polaridad en la salida, mientras que una entrada aplicada a la terminal inversora aparecerá invertida en la salida. 

Como elemento activo, es necesario un suministro de tensión al amplificador operacional, como se muestra del modo común en la figura:

![](https://github.com/erickfi/practica-8/blob/master/Imgs/alimentacion%20del%20amplificador.PNG)

En una idea simplificada se puede decir que el amplificador operacional es un circuito integrado cuya principal función es amplificar el voltaje con una entrada de tipo diferencial para tener una salida amplificada y con referencia a tierra. Existen dos configuraciones que puede adoptar un amplificador, lazo abierto y lazo cerrado.

##### CONFIGURACIÓN DEL AMPLIFICADOR OPERACIONAL EN LAZO ABIERTO

En esta configuración partimos de que la ganancia esta ajustada a un valor muy alto (aproximadamente 200,000 veces). Esta ganancia el lazo abierto se le conoce como AOL y esta en función a la diferencia de las entradas del Op-Amp. La ganancia en lazo abierto es la salida máxima que se puede obtener del amplificador operacional.

El voltaje de saturación en un amplificador operacional es un «poco» menor que el voltaje de la fuente. Esta caída de voltaje depende del fabricante.

Una de las aplicaciones mas recurrentes de esta configuración es como comparador, en este caso se deja una de las entradas con un voltaje fijo. Usualmente, el voltaje configurado con un divisor de voltaje para tener una referencia. Y la otra entrada conectada a la salida de un sensor. En este caso podemos tener un sistema que tenga una salida activada pasando este umbral. Esta configuración es muy útil ya que no depende de un sistema inteligente como un microcontrolador.

Al analizar el circuito, podemos obtener el voltaje de salida mediante la siguiente fórmula.

![](https://github.com/erickfi/practica-8/blob/master/Imgs/voltaje%20de%20salida%20en%20lazo%20abierto.PNG)

##### CONFIGURACIÓN DEL AMPLIFICADOR OPERACIONAL EN LAZO CERRADO (GANANCIA CONTROLADA)

Un amplificador operacional o opamp en ganancia controlada, considera una retroalimentación de la salida respecto a la entrada. Las dos configuraciones más básicas son la del inversor y no inversor. Otras configuraciones se detallaran en otros tutoriales más adelante.

##### Retroalimentación

El concepto de retroalimentación es crucial para la comprensión de los circuitos de amplificadores operacionales. 

Una retroalimentación negativa se obtiene cuando la salida se retroalimenta a la terminal inversora del amplificador operacional, cuando hay una vía de retroalimentación de la salida a la entrada, la proporción entre la tensión de salida y la tensión de entrada se llama ganancia de lazo cerrado. Como resultado de la retroalimentación negativa, es posible demostrar que la ganancia de lazo cerrado es casi insensible a la ganancia de lazo abierto A del amplificador operacional. Por esta razón se usan amplificadores operacionales en circuitos con trayectorias de retroalimentación.

Una limitación práctica del amplificador operacional es que la magnitud de su tensión de salida no puede exceder de |VCC|. En otras palabras, la tensión de salida depende de y está limitada por la tensión de alimentación. La figura ilustra que el amplificador operacional puede funcionar en tres modos, dependiendo de la tensión de entrada diferencial vd.

![](https://github.com/erickfi/practica-8/blob/master/Imgs/tension%20de%20salida.PNG)

Si se intenta incrementar vd más allá del rango lineal, el amplificador operacional se satura y produce vo=VCC ó vo=-VCC.

### 4. DIAGRAMAS
**Diagrama del circuito**

![](https://github.com/erickfi/practica-8/blob/master/Imgs/diagramas%20de%20circuitos.PNG)

**Construcción del diagrama en Proteus**

![](https://github.com/erickfi/practica-8/blob/master/Imgs/diagramas%20proteus.PNG)

**Simulación**
##### Circuito 1 

![](https://github.com/erickfi/practica-8/blob/master/Imgs/circuito%201.PNG)

##### Circuito 2

![](https://github.com/erickfi/practica-8/blob/master/Imgs/CIRCUITO%202.PNG)

##### Circuito 3

![](https://github.com/erickfi/practica-8/blob/master/Imgs/circuito%203.PNG)

### 5. LISTA DE COMPONENTES




### 6. PREGUNTAS

***Anote parámetros técnicos importantes de un amplificador operacional que deben ser tomados en cuenta al momento de utilizarlos en un proyecto.***

> Los parámetros a tener en cuenta para implementar un amplificador operacional en cualquier circuito electrónico son:

> - La Impedancia de Entrada y Salida

> Son las resistencias que se encuentran conectadas a la entrada y salida del amplificador. 

> - Tensión de Alimentación

> Es la tensión máxima permitida y que es aplicada en los terminales de entrada diferencial sin flujo excesivo de corriente.

> - Tensión de Entrada diferencial

> Es la tensión máxima permitida y que es aplicada en los terminales de entrada diferencial sin flujo excesivo de corriente.

> - Tensión en Modo Común 

> Es el rango de voltaje aplicable en ambas entradas con respecto a tierra.

> - Consumo y Disipación de Potencia

> En el consumo se tiene una potencia requerida para operar un amplificador operacional con propósitos de polarización, en disipación se tiene una potencia en la cual un dispositivo es capaz de disipar de manera segura y continua mientras otro opera dentro de un rango de temperatura específico.

> - Rango de Temperaturas de Operación

> Es el rango de temperatura donde el dispositivo funciona bajo las especificaciones requeridas.

***Investigue las características de amplificadores operacionales distintos a los utilizados en esta práctica.***

> Los operadores utilizados en esta práctica fueron el LM3424J y el 741, sin embargo, existen muchos otros amplificadores muy utilizados actualmente en la industria debido a las características que poseen, como por ejemplo:

> -Los (opamps), se encargan de amplificar la tensión, suelen ser los bloques de construcción de sistemas electrónicos en un amplio rango de dispositivos y equipos. También existen los nuevos (opamps) capaces de trabajar a 200mV por debajo de cero en modo común, incrementando la libertad de diseño al poder resistir hasta 6 V con la máxima ratio y ampliando el margen de un fuente típica de 5 V.

> -TSV85x y LMV82x, convierten en una actualización del estándar de la industria LMV321 para aplicaciones de acondicionamiento de señal informática, sanidad e industria. Estos amplificadores operacionales cuentan con una opción de pin shut-down que ayuda a minimizar el consumo de corriente a "prácticamente cero" y las versiones de grado A ofrecen los valores más bajos de tensión offset de entrada.

***Investigue otras aplicaciones con circuitos más complejos que utilizan amplificadores operacionales.***

> Las aplicaciones de los OP son muy extensas y diversas, entre las numerosas aplicaciones prácticas tenemos: 

> Amplificadores para instrumentos, convertidores digitales-analógicos, computadoras analógicas, cambiadores de nivel, filtros, circuitos de calibración, inversores, sumadores, integradores, diferenciadores, restadores, amplificadores logarítmicos, comparadores, elementos rotatorios, osciladores, rectificadores, reguladores, convertidores de tensión a corriente, convertidores de corriente a tensión y recortadores.
### 7. ANÁLISIS DE RESULTADOS

Al observar las gráficas de los circuitos podemos observar la gráfica del circuito 1 y el circuito 3 son similares esta similitud se debe a los componentes que tienen, ya que ambas se componen únicamente de resistores, y su diferencia radica en las fuentes y la forma en la que se conectan estas, reforzando el pensamiento de que un amplificador nos da resultados distintos dependiendo de como se conecten e interactúen sus elementos.

Al comparar las gráficas 1, 3 y 2, notamos una gran diferencia, y no precisamente en la forma de la gráfica, sino en la representación de la misma, para las graficas 1 y 3, se nota que existe una simetría, desde que va de un valor 0 V al voltaje máximo, mientras que la grafica 2 nos da una gráfica que no es simétrica, por lo que tenemos voltajes variados, esto es debido a que este circuito tiene conectado un capacitor en el retorno en el lugar de una resistencia lo que hace que se genere una onda de esa forma.

Observando las gráficas, que nos dan el voltaje de salida, y comparando con los voltajes de entrada, tenemos que este se amplifica en razón de 4.3 veces el valor de entrada, cumpliendo así con la función del amplificador operacional que es aumentar el voltaje.

### 8. CONCLUSIONES

> En el primer circuito se observó una amplificación o incremento en el voltaje proporcionado por la fuente de voltaje AC de 1V, este incremento esta dado en un factor de 4.3 veces el voltaje de entrada, y esto es debido precisamente a la configuración del circuito, el amplificador operacional LM324J es alimentado por las terminales 4 y 11 con un voltaje de 14 V y dado que las resistencias de entrada y salida son 1k y 4.3 k ohmio respectivamente, se logra amplificar el voltaje de entrada de nuestro circuito.

> El segundo circuito es conocido como integrador, debido a que la señal de salida en verdad es la integral de la función de entrada, esto se lo comprueba al analizar la integral de la señal de entrada, que es una constante que cambia en un periodo dado por lo que su integral también de entrada se dará por partes, entonces la gráfica de la antiderivada de la señal de entrada es una cierra, esto debido a que en la integral de una constante es una línea recta que tiene como pendiente esta constante siendo esa en nuestro caso el voltaje pico de 5 voltios, y al cambiar esta periódicamente entre positivo y negativo, la pendiente en la señal de salida también cambiara de creciente a decreciente, por último se observa que este cambio es inverso ya que cuando la señal de entrada es positiva la pendiente es decreciente.

> En el tercer circuito al igual que el primero, se obtiene un incremento sobre el voltaje de entrada, en este caso la configuración del circuito al tener dos fuentes de voltaje de corriente alterna en paralelo, el factor de incremento en el voltaje de salida esta relacionado directamente con dichas fuentes y sus respectivas resistencias conectadas en serie, y como también la resistencia de salida. Obteniendo un voltaje de salida de 8,33 V.

### 9. RECOMENDACIONES

- Usar el amplificador específicado, ya que existen diferentes tipos y cada uno da un resultado diferente aún si se realiza una misma conexión.
- Conectar la fuentes según lo indica el diagrama, si se conectan del polo opuesto los resultados vana  variar.
- Variar las fuentes ayudará en la comprensión de como funciona el amplificador operacional.

### 10. CRONOGRAMA

![](https://github.com/erickfi/practica-8/blob/master/Imgs/Cronograma-8.PNG)

### 11. REFERENCIAS
- [1] M. A. Sadiku.Fundamentos de circuitos eléctricos. Mc Graw Hill, third edition, 2006
### 12. ANEXOS

- [Cálculos](https://github.com/erickfi/practica-8/blob/master/Anexos/Anexos.pdf)
- [Cómo se implementó el circuito](https://youtu.be/wuU_yvoSkqg)
- [Cómo funciona el circuito](https://youtu.be/n54IluLJb14)
