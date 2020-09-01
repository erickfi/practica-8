## UNIVERSIDAD DE LAS FUERZAS ARMADAS ESPE
![](https://github.com/erickfi/Practica-5/blob/master/Img/Escudo.jpg)
### Práctica de laboratorio N° 7
## Características de la onda senoidal
**Autores:** Figueroa Erick, León Jipshon,Viracucha William.
### 1. PLANTEAMIENTO DEL PROBLEMA

En estudio de la corriente eléctrica se divide en dos grupos, por un lado está la corriente directa DC, y por el otro la corriente alterna AC, aunque los teoremas y principios eléctricos se aplican a ambos tipos, su estudio difiere por las características que los componen, es por ello que su aplicación es muy diversa, por lo general, la corriente continua se usa para elementos del diario vivir, celulares, portatiles, y se la suele atribuir con una batería, mientras que la corriente alterna la encontramos en los cables de alta tensión, y en los medidores eléctricos de nuestras casas.

Una de las principales diferencias entre la corriente alterna y la corriente continua es la intensidad en las que se presentan, siendo la intensidad de corriente su principal diferencia donde la corriente alterna es mucho mayor que la corriente continua, es por ello que dentro de la ingenieria existen dos ramas distintas para el estudio y trabajo con las mismas, la energia electrónica para la corriente continua y la ingenieria eléctrica para la corriente alterna

### 2. OBJETIVOS
#### Objetivo General

- Determinar experimentalmente las características de señales senoidales.

#### Objetivos Específicos
- Entender el funcionamiento del osciloscopio.
- Analizar la senoide que forma el voltaje en una resistencia.
- Comparar el voltaje maximo de la senoide con el obtenido con un voltímetro en C.A.
### 3. MARCO TEÓRICO

Las ondas senoidales son patrones de ondas que matemáticamente pueden ser descritas mediante las funciones seno y coseno. Describen acertadamente eventos naturales y señales variables en el tiempo, tales como los voltajes generados por centrales eléctricas y luego utilizados en hogares, industrias y calles.

El libro _Fundamentos de circuitos eléctricos_ (Sadiku, 2006) nos dice:
> Una senoide es una señal que tiene la forma de la función seno o coseno.

Las ondas senoidales nos permiten describir diversos fenómenos físicos con una notable precisión, al estudiar la eléctricidad la onda senoidal se usa para describir la forma que adopta la corriente alterna si la conectamos a un osciloscopio. Una corriente senoidal se conoce usualmente como corriente alterna (ca). Esta corriente se invierte a intervalos regulares y tiene valores alternadamente positivo y negativo. Los circuitos excitados por fuentes de corriente o tensión senoidal se llaman circuitos de ca.

La corriente alterna tuvo su aparición al finales de siglo XIX, siendo Nikola Tesla (1856-1943) uno de los principales defensores de esta una forma de corriente.

> La contribución más significativa a los primeros éxitos de la ca fue la patente lograda por Tesla en 1888 del motor polifásico de ca. El motor de inducción y los sistemas polifásicos de generación y distribución sentenciaron a muerte el uso de la cd como fuente primaria de energía.

Al estudiar los circuitos de corriente continua llegamos a la indudable conclusión de que los elementos del circuito son existados por la fuente del circuito, sea de corriente o de voltaje, en la corriente alterna ocurre lo mismo, sin embargo, ya que su fuente es una onda senoidal, es necesario conocer las carácterísticas de la misma.

**Función Coseno**

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/funci%C3%B3n%20cos.jpg)

**Función Seno**

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/funci%C3%B3n%20seno.jpg)

Ambas gráficas corresponden a ondas senoidales, generalmente se usa la _función Coseno_ al momento de trabajar con circuitos ac, pero, esto no quiere decir que la _función Seno_ no se presente en algún análisis, ya que ambas describen ondas senoidales, se las considera complementarias, es decir, similares por lo que comparten las mismas características.

#### Características de la onda senoidal

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/partes.png)

Onda senoidal representa el valor de la tensión de la Corriente alterna a través de un tiempo continuamente variable, su representación en el plano cartesiano viene dado por la amplitud y el tiempo. Una onda senoidal es periódica y cuenta con los siguientes elementos:

- **Periodo:** Intervalo de tiempo donde la onda realiza un ciclo.   
- **Frecuencia:** Número de ciclos que tienen lugar en la unidad de tiempo y se determina como el inverso del periodo (1/T).
- **Amplitud:** Es el valor de los extremos, valles y crestas, que la onda alcanza.

#### Representación matemática de una onda senoidal

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/representacion%20Math.PNG)

### 4. DIAGRAMAS
**Diagrama del circuito**

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/diagrama.PNG)

**Construcción del diagrama en Proteus**

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/osciloscopio%20proteus.PNG)

**Simulación**

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/simulacion%201.jpeg)

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/simulacion%202.jpg)

### 5. LISTA DE COMPONENTES

![](https://github.com/erickfi/Laboratorio-7/blob/master/Imagenes/componentes.PNG)

### 6. PREGUNTAS

***¿Cuántas divisiones por cuadro abarca la amplitud pico de la señal de salida?***

	6

***¿En qué valor está posicionada la perilla VOLTS/DIV?***

	1.15 V

***¿Cuántas divisiones por cuadro abarca un ciclo completo de la señal de salida?***

	8

***¿En qué valor está posicionada la perilla TIME/DIV?***

	50 us

***¿Cuál es la amplitud de voltaje y el periodo de la señal que aparece en la pantalla del osciloscopio?***

	Amplitud de voltaje: 6.9 (V) 
	Período:  0.0004 (s) 

**Determine la frecuencia natural (Hz) y la frecuencia angular (rad/s) de la señal de salida.***

	f: 2.5 k   (Hz) 
	ω: 5000 π  (rad/s) 
	
***Con el multímetro digital mida el voltaje de salida en RL:***
	
	4.86 V

***Compare el voltaje medido en el punto 7.5.5. y el obtenido en el punto ¿Coinciden? ¿Por qué?***

	El valor obtenido en el osciloscopio es 6.9 V y el medido por el multímetro es 4.86 V, no coinciden por el hecho que el osciloscopio
	nos entrega el valor pico del voltaje y el multímetro el valor rms, entonces si dividimos el voltaje pico de 6.9 V para la raíz de 
	dos obtenemos un valor de 4.879 V, siendo este un valor próximo a 4.86 V, verificando así que el valor medido con el multímetro 
	efectivamente es el valor eficaz o rms del voltaje que pasa por la resistencia de 2.2k ohmios.


### 7. CONCLUSIONES
- El osciloscopio nos permite medir el voltaje máximo de un componente de un circuito de corriente alterna, mientras que el multimetro nos dará el valor del voltaje eficaz Vrms.
- Se puede aproximar el voltaje máximo de un elemento con la gráfica del osciloscopio, dando a cada cuadro un valor de voltaje y ajustando el número de cuadros a la imagen que nos da el osciloscopio.
- El valor máximo que alcanza un circuito no será el mismo que existará a los elementos, para ello se usa el voltaje eficaz y la variación de ambos es en un factor igual a la raíz cuadrada de 2.
- Como se puede observar en los resultados la frecuencia queda inalterada, es decir sigue siendo 2.5khz, pero el voltaje sufre una reducción a 6.9v de 10 del valor de voltaje máximo, por lo que la frecuencia debe ser constante en todo el circuito.
- Hay un error del 0.4% por lo que el valor de lectura del multimetro es muy parecido a la precisión que nos da el oscilador.

### 8. RECOMENDACIONES

- Buscar el simulador adecuado, donde los componentes del software permitan simular corriente alterna y que tenga un osciloscopio que permita obervar de manera correcta a la onda.
- El osciloscopio debe tener una referencia a tierra para ser usado, ya que en corriente alterna no existe polaridad y por lo tanto no entregaría los valores que se estan buscando.
- Se debe diferenciar entre el voltaje eficaz, voltaje máximo, y voltaje pico a pico, para evitar un mal cálculo y evitar asi resultados falsos lo cual puede generar serios problemas.


### 9. CRONOGRAMA
![](Imagenes/Cronograma-Practica-7.PNG)


### 10. REFERENCIAS
- [1] M. A. Sadiku.Fundamentos de circuitos eléctricos. Mc Graw Hill, third edition, 2006
### 11. ANEXOS

- [Cálculos](https://github.com/erickfi/Laboratorio-7/blob/master/Anexos/LAB_7_CIRCUITOS.pdf)
- [Cómo se implementó el circuito](https://youtu.be/wFO5DdxBPt8)
- [Cómo funciona el circuito](https://youtu.be/656tT3m5qm4)
