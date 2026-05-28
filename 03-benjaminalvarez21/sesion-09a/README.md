# sesion-09a

Clase online por incendio al lado de la u :c

En esta clase repasamos algunas que vimos en la clase 08a que se trató de Kicad y aparte vimos más de como hacer la PCB. La clase anterior habíamos llegado hasta solo pasar los componentes a la sección de PCB, así que aparte de repasar, vimos desde el paso 4 al paso final.

Importante, tener noción del tamaño de la grilla en la que trabajamos, mientras más pequeña, es más precisa y tiene más resolución.

Antes de comenzar con los pasos, generamos el contorno de la PCB con el que tenemos que trabajar que es de 90 x 50 mm.

## Paso 4 Definir pistas

Hay dos capas de cobre que son las pistas, las pistas son cables con lo que se conectan los componentes en la PCB. Mientras más gruesa la pista fluye más corriente. Las pistas equivalen a los cables dupont que usamos en la construcción física con las protoboards.

Utilizamos pistas de 0.4mm para las conexiones entre componentes, y usamos pistas de 0.8mm para el vcc.

Las pistas se parecen a las líneas del metro.

## Paso 5 Distribución de componentes

Este paso consiste en ordenar los elementos que pusimos en el esquemático, pero ahora en la PCB, hay que tener en cuenta algunas reglas como poner los componentes no pegados entre ellos y mantener orden, así se nos va a facilitar después la conexión. Todos estos componentes van dentro del margen que creamos al inicio.

## Paso 6 Rutear conexiones

Aquí se realizan las conexiones entre los componentes que ordenamos en la PCB usando los dos pinceles que guardamos antes. Hay que tener ojo porque cuando trabajamos en una capa las pistas pueden chocar entre sí, así que ahí tenemos dos opciones, usar la otra capa para pistas o utilizar vías que son puentes que pasan de una capa a otra. Estas se crean con la tecla V cuando estás dibujando una pista.

Para conectar GND, hay una opción que la crea automáticamente, tenemos que crear una zona que cubra toda la PCB, tenemos que elegir la herramienta que se llama dibujar zonas rellenas, seleccionamos que queremos rellenar las dos capas de las pistas, elegimos la red GND y dibujamos sobre la PCB. Da igual que no sea preciso este paso, funcionará igual. Al tener seleccionada la zona, confirmamos y apretamos la tecla B, esto rellenará todo.

## Paso 7 Preparar fabricación

Este es el último paso, acá tenemos que darle los detalles finales a la PCB como los agujeros de montaje o diseños gráficos que nosotros queremos darle a la PCB.

Para agregar los agujeros tenemos que pasar al esquemático y agregar MountingHole, estos sirven para poder fijar la placa con tornillos. Tenemos que poner valor y huellas. Le ponemos valor M3 y la huella MountingHole:MountingHole_3.2mm_M3. 

Y como detalles finales podemos poner diseños, imágenes o textos, pueden ser formato SVG o DFX. Para importarlo tienes que apretar Archivo, luego Importar y después Gráficos. Hay que fijarse que esté en mm y siempre hacerlo en la capa Silkscreen.

## Encargo

En este encargo nos pidieron hacer dos placas de dos procesos distintos de los sintetizadores que hicimos en la primera entrega y aparte leer el capítulo 1 del libro Hacia una filosofía de la fotografía de Vilém Flusser.

Link del libro:

<https://monoskop.org/images/8/8d/Flusser_Vilem_Hacia_una_filosofia_de_la_fotografia.pdf>

### Primera placa 555 CLOCK

Primero escogí hacer la placa del 555, se hizo un poco lento ya que fue el primero que hice solo pero se logró, aca hay distintas capturas:

### Esquemático

Esta parte fue fácil ya que es sólo ordenar las piezas corrector en el orden correcto.

![esquemático 555](./imagenes/555-esquematico-pescado.png)

### Huellas utilizadas para CLOCK 555 del encargo

La parte más tediosa a mi parecer, ya que el ir buscando las huellas y corroborar que están bien no me gusto nada, aquí una imagen de las huellas en el Kicad y aparte el listado escrito. 

![huellas 555](./imagenes/huellas-555.png)

Condensador cerámico: Capacitor_THT:C_Disc_D3.8mm_W2.6mm_P2.50mm

Condensador electrolítico 10u: Capacitor_THT:CP_Radial_D5.0mm_P2.00mm

Resistencia: Resistor_THT: R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal

555: Package_DIP:DIP-8_W7.62mm_LongPads

Potenciómetro: Potentiometer_THT:Potentiometer_Alps_RK163_Single_Horizontal

Botón: Button_Switch_THT:SW_PUSH_6mm

Tornillo: MountingHole:MountingHole_3.2mm_M3

Led: LED_THT:LED_D5.0mm

Batería: TerminalBlock:TerminalBlock_MaiXu_MX126-5.0-02P_1x02_P5.00mm

### PCB con pistas y vista 3d

La parte de las pistas pensé que iba a ser complicada pero terminó siendo fácil, solo hay que tener ojo de que estén bien hechas. Aquí foto de la PCB con las pistas y también de cómo se vería en 3d.

### Foto PCB

![esquemático 555](./imagenes/555-esquematico-pescado.png)

### Fotos 3d

![3d 555](./imagenes/3d-pcb-555.png)

![3d 555](./imagenes/3d-pcb-555-back.png)

Mi placa six seven

### Segunda Placa LM 386

Aca segui el mismo proceso pero con los componentes de el LM 386 asi que solo dejare las fotos.

### Esquemático

![esquemático lm386](./imagenes/lm386-esquematico.png)

### Huellas usadas para MIX del encargo

![huellas lm386](./imagenes/huellas-lm386.png) 

Condensador cerámico: Capacitor_THT:C_Disc_D3.8mm_W2.6mm_P2.50mm

Potenciómetro: Potentiometer_THT:Potentiometer_Alps_RK163_Single_Horizontal

Tornillo: MountingHole:MountingHole_3.2mm_M3

Batería: TerminalBlock:TerminalBlock_MaiXu_MX126-5.0-02P_1x02_P5.00mm

Parlante: TerminalBlock:TerminalBlock_MaiXu_MX126-5.0-02P_1x02_P5.00mm

Condensador electrolítico 100u: Capacitor_THT:CP_Radial_D6.3mm_P2.50mm

### PCB con pistas y vista 3d

![pcb lm386](./imagenes/pcb-lm386.png)

![3d lm386](./imagenes/3d-pcb-lm386.png)

### Reflexión capítulo 1

Al empezar a leer el texto, realmente me costó, no estaba entendiendo mucho de este y se me estaba haciendo un poco enredado. Así que me puse a leer la nota introductoria antes del capítulo y entendí que es un libro muy hipotético que lleva a la discusión sobre el tema principal que es la fotografía, pero más bien de un lado más filosófico.

Es interesante el cómo presenta la imagen, como algo imaginativo y dentro de le encuentro un poco de razón, porque las imágenes es el momento congelado de una situación la cual sucedió en algún momento pero para poder adivinar o poder analizar que sucedió en este entonces, tenemos que usar nuestra imaginación y hacer nuestra propia interpretación de lo que creemos que pasó. Aunque el texto diga que no son eventos congelados, no estoy de acuerdo porque en parte lo son pero eso no quita que dejemos la magia y el poder de la imaginación atrás.

Cuando empieza a hablar de este mundo dominado por imágenes y que el humano vive a partir de ellas llamando idolatría, no se porque pero me hizo relacionarlo un poco a situaciones que se pueden ver en la actualidad, en como mucha gente vive en las redes sociales y a partir de imágenes que comparten y siento que no son nada sin ellas, que pierden su identidad si no están constantemente compartiendo imagenes. Me llama la atención cómo comparar épocas antiguas y que viven una situación similar con el texto y que pierden lo que es la magia ya que rigen su vida por el texto el cual ya viene totalmente estructurado, yo siento que el texto igual tiene algo de imaginación, algo de magia. Siento que un cuento, una novela, requiere imaginación, claramente para crear la imagen de como ficticiamente este texto podría verse de manera física.

Terminando el capítulo, siento que la imagen es un buen incentivador de la imaginación, pero no descarto que el texto también lo sea, pero siento que si quieres darle magia a un texto, si o si tiene que haber una imagen de por medio, aunque venga de la imaginación.
