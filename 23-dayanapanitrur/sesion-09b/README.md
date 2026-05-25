# sesion-09b

## Apuntes de la clase

Misaa dejó un glosario de Kicad que hizo hace un tiempo para todos estos conceptos, que normalmente ahora que estamos iniciando son complejos de entender.

El dip-16 de 7.62 de mm es el más común | DIP - NÚMERO DE PATAS - LONGPADS (Para Misaa esta es una de las mejores opciones porque son más faciles de soldar ya que las patas son más anchas).
Para el momento en el que queramos actualizar huellas no se actualiza automáticamente: 
Desde el CI se le da a F (propiedades) y se empieza a modificar. Luego se le da a actualizar desde el esquemático hacia la placa, esa opción donde aparecen dos imagenes divididas en una diagonal.

Biblioteca de símbolos.
Hay ciertos símbolos que ya existen en el mundo de Kicad y que al momento de editarlos directamente (Editar símbolo de biblioteca) los podemos descomponer. Y eso significa PELIGRO. Importante no hacer.

Apretando la letra E se les puede editar ciertas elementos visuales, como el color de un chip por ejemplo. No soy muy fan del amarillo *post it* tampoco.

PIN + M > así podemos cambiar el pin 5 del chip 555 que está conectado a tierra pero por alguna razón en default está ubicado arriba (esa ubicación nada que ver) y ahí también podemos dejarle otro llamado como CV, no de curriculum vitae sino de Control Voltage.

Ya pasamos por pcb y sch

y ahora podemos abrir editor de símbolos (triangulo azul con patitas en mi cabeza)
de ahí para no trabajar en el aire obviamente se puede crear una biblioteca.

Archivo> nueva biblioteca: Para crear una biblioteca en la cual pueda guardar mis símbolos.
Y desde aquí puedo editar los símbolos sin dañar los de la biblioteca original.

* Están los botones temporales o pulsadores

El más común es el N O (normaly open)

Se utiizan para distintas gestualidades

Un piano utiliza un pulsador

La lámpara de mi pieza utiliza un swtich

Los botones de pedalera se llaman 3PDT y también son switch

* Lo más probable es que utilicemos un SPDT para no tener que estar conectando y desconectando la batería.

Para colocar esas conexiones (tipo etiquetas) sin tener que mandar el cable completo, para indicar que allí hay una conexión: ejemplo para no tener que conectar step por step y así.
Se puede hacer mediante un simbolo en el browser a la derecha que tiene una letra A y un _ abajo de esta. Colocar etiquetas de red o también con la tecla (L) directamente.

En propiedades de huellas se puede modificar o integrar modelos 3d (por ejemplo descargando un modelo de potenciómetro en internet, ya que este no aparece en la placa).
