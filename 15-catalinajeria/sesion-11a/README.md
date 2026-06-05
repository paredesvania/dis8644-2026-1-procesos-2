# Clase 11a — Filtros activos, KiCad y Flusser

**Tema:** esquemático en KiCad, filtros activos y capítulos 8 y 9 de Flusser  
**Trabajo de clase:** pruebas con LM324, LM358 y filtro Sallen-Key

---

## Resumen de la clase

En esta clase seguimos trabajando en KiCad, pero ahora enfocados en el diseño de filtros activos. La idea era empezar a probar circuitos que nos permitieran filtrar señales, especialmente para separar o modificar frecuencias dentro de un proyecto sonoro.

Durante la clase hicimos pruebas con amplificadores operacionales como el **LM324** y el **LM358**, pensando en usarlos para construir filtros activos de paso bajo y paso alto. La idea era ver cómo estos integrados podían ayudarnos a controlar qué frecuencias pasan y cuáles se atenúan.

También trabajamos tomando como referencia el esquemático del profesor Misa. Desde ahí intentamos entender mejor cómo estaba armado el circuito y qué partes podían servirnos para nuestro propio filtro.

---

## Trabajo en KiCad

En KiCad comenzamos a armar el esquemático del circuito. La idea era pasar desde una idea más teórica del filtro hacia algo más concreto, donde pudiéramos ver los componentes, sus conexiones y la posible estructura del circuito.

El trabajo principal fue ordenar el esquemático y probar distintas posibilidades para el filtro. En esta etapa todavía no se trataba de llegar a la placa final, sino de entender cómo conectar los componentes y cómo se podía comportar el circuito.

---

## Filtros activos

Un filtro activo es un circuito que usa componentes pasivos, como resistencias y capacitores, junto con un componente activo, normalmente un amplificador operacional.

La gracia de usar un operacional es que el filtro no solo deja pasar o corta frecuencias, sino que también puede ayudar a estabilizar, amplificar o controlar mejor la señal.

En la clase estuvimos pensando principalmente en dos tipos de filtros:

- **Filtro paso bajo:** deja pasar frecuencias bajas y atenúa las altas.
- **Filtro paso alto:** deja pasar frecuencias altas y atenúa las bajas.

Esto era importante porque queríamos encontrar una forma de controlar mejor el sonido y separar rangos de frecuencia.

---

## Integrados usados

Los integrados que revisamos fueron principalmente:

| Integrado | Uso pensado |
|---|---|
| `LM324` | Amplificador operacional cuádruple, útil para probar varias etapas de filtro. |
| `LM358` | Amplificador operacional doble, más simple para pruebas iniciales. |

El **LM324** puede ser útil cuando se necesitan varias etapas dentro del mismo circuito, porque trae cuatro amplificadores operacionales en un solo chip. El **LM358**, en cambio, trae dos, por lo que puede ser más cómodo para probar un filtro más pequeño o una parte específica del circuito.

---

## Búsqueda del filtro Sallen-Key

El profesor nos pidió revisar el filtro **Sallen-Key**, porque es una configuración muy usada para hacer filtros activos de segundo orden.

Este tipo de filtro usa un amplificador operacional junto con resistencias y capacitores. Se puede usar para armar filtros paso bajo o paso alto, dependiendo de cómo se ordenen los componentes.

En esta clase lo revisamos como una posible base para nuestro diseño, ya que necesitábamos lograr un filtro activo que pudiera trabajar con frecuencias altas y bajas.

---

## Idea general del filtro Sallen-Key

El filtro Sallen-Key sirve para construir filtros activos de manera relativamente simple. Normalmente se usa con un amplificador operacional configurado como buffer o seguidor de voltaje.

La idea general es que las resistencias y capacitores definen la frecuencia de corte, mientras que el operacional ayuda a mantener la señal y darle estabilidad al circuito.

En el caso del filtro paso bajo, las frecuencias bajas pasan hacia la salida y las frecuencias altas se van atenuando. Esto nos sirve si queremos suavizar una señal o eliminar partes muy agudas.

---

## Lo que quedó pendiente

En esta clase no logramos cerrar completamente el diseño del filtro, pero sí avanzamos en entender qué necesitábamos probar.

Quedó pendiente:

- Revisar mejor el filtro Sallen-Key.
- Definir si nos conviene usar LM324 o LM358.
- Entender bien la diferencia entre paso alto y paso bajo en el esquemático.
- Probar si el circuito del profesor Misa se puede adaptar a nuestro proyecto.
- Ver cómo llevar el filtro a una versión más concreta en KiCad.

---

# Resumen de Flusser — Capítulos 8 y 9

## Capítulo 8 — El universo fotográfico

En este capítulo, Flusser habla del mundo lleno de fotografías en el que vivimos. Explica que estamos tan acostumbradas a ver imágenes por todas partes que muchas veces ya ni las notamos. Las fotos cambian todo el tiempo en diarios, carteles, pantallas y publicidad, pero ese cambio constante ya se volvió parte de lo cotidiano.

La idea principal es que el universo fotográfico no solo muestra imágenes, sino que también programa nuestra forma de mirar y actuar. Flusser dice que muchas fotografías son redundantes, porque se reemplazan unas a otras sin aportar algo realmente nuevo. Siempre aparece una imagen nueva, pero muchas veces cumple la misma función que la anterior.

También habla de cómo los colores y las imágenes del mundo actual funcionan casi como una contaminación visual. Estamos rodeadas de estímulos que parecen normales, pero que igual influyen en nuestra conducta. Por ejemplo, un color como el rojo puede activar una reacción automática, como detenerse en un semáforo.

Flusser plantea que el universo fotográfico está formado como un mosaico de puntos o fragmentos. Esto se conecta con la lógica de los aparatos, porque estos funcionan mediante programas, combinaciones y elementos separados. En ese sentido, la cámara y otros aparatos no producen imágenes inocentes, sino imágenes que responden a un programa.

El problema es que este universo puede transformar a las personas en funcionarias de los aparatos. Es decir, en vez de usar los aparatos libremente, terminamos actuando según lo que ellos permiten o programan.

En resumen, el capítulo muestra que vivimos dentro de un universo de imágenes técnicas que se actualizan constantemente, pero que muchas veces repiten lo mismo. Para Flusser, el desafío está en producir imágenes realmente informativas, que no sean solo otra repetición dentro del programa.

---

## Capítulo 9 — La necesidad de una filosofía de la fotografía

En este capítulo, Flusser explica por qué es necesaria una filosofía de la fotografía. Para él, no basta con mirar fotografías o estudiar su historia; también hay que pensar qué significan dentro de una sociedad dominada por aparatos.

Flusser resume varios conceptos importantes del libro: imagen, aparato, programa e información. Estos conceptos sirven para entender que la fotografía no es solo una imagen, sino el resultado de un aparato automático que funciona según un programa.

Una idea importante es que la fotografía cambia la forma en que pensamos. Ya no vivimos solamente en una historia lineal de causa y efecto, sino en un mundo más parecido a un juego de combinaciones. Los aparatos repiten, combinan y producen posibilidades, muchas veces sin una intención humana clara.

Por eso aparece el problema de la libertad. Si los aparatos ya están programados y nos hacen actuar dentro de sus posibilidades, entonces la pregunta es: ¿dónde queda la libertad humana?

Flusser cree que los fotógrafos experimentales pueden dar una pista. Ellos intentan jugar contra el aparato, producir imágenes que no estaban previstas y usar la cámara de una manera menos automática. En ese gesto aparece una posibilidad de libertad.

En resumen, Flusser plantea que necesitamos una filosofía de la fotografía para entender cómo los aparatos nos programan, pero también para buscar formas de actuar creativamente dentro de ese mundo. La libertad no estaría en ignorar los aparatos, sino en aprender a jugar contra ellos.

---

## Reflexión personal

Esta clase conectó bien la parte técnica con Flusser. Por un lado, estábamos trabajando con filtros, operacionales y esquemáticos en KiCad. Por otro lado, Flusser habla de los aparatos como sistemas que reciben una entrada, procesan algo y entregan una salida.

Pensándolo así, una cámara, un escáner o incluso un circuito con un LM324 también pueden entenderse como aparatos. Todos transforman algo: luz, sonido, voltaje o información.

Me quedó la idea de que no basta con usar un circuito o una herramienta. También hay que entender qué hace, qué limita y qué posibilidades abre. En nuestro caso, el filtro no solo modifica una señal: también define qué parte del sonido queremos dejar pasar y qué parte queremos cortar.

Por eso, trabajar con filtros también es una forma de tomar decisiones sobre cómo queremos escuchar o construir una señal.
