# sesion-09a

## Kikad (Clase online)

### 1era Parte
+ Repaso clase anterioir + comandos a destescar ( Incoportado en sesión 8a)

### 2da Parte (placa PCV)

Clase anterior:
![interfas-placa](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/ff35bf81028fffec49ba106a396c1226e377e589/12-paulafuentesm/sesion-09a/imagenes/interfas-placa.png)

#### Capas:
+ Edge.cuts: Donde se dibuja la placa
+ F.Cu:cables ( pistas de entre 0,3 a 0,4)-ocupada 0.8
+ B.Cu: cables si es que chocan en la capa F.cu ( pistas de entre 0,3 a 0,4)- ocupada 0.4
+ F. silkscreen: dibujar o serigrafiar
+ Mask: guías

**Importante:** Sí es que chocan los cables igualmente en la capa B.Cu, apretar V para ir tejiendo entré capasa

Placa:
![placa](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/92869b8e473a1e99843328a10dc4171e1480fafd/12-paulafuentesm/sesion-09a/imagenes/placa.png)

Placa 3D:
![placa3d](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/92869b8e473a1e99843328a10dc4171e1480fafd/12-paulafuentesm/sesion-09a/imagenes/placa3d.png)

Error (preguntar Viernes):
![error1](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/92869b8e473a1e99843328a10dc4171e1480fafd/12-paulafuentesm/sesion-09a/imagenes/error1.png)

+ puede ser que en algùn momento conte los cables y quedo pero no se vé
+ no entiendo si es que dice error en la pata 1 del chip, cuando ese va conectado a GND
+ me falto colocar el led para ver si estaba encendido el circuto, no olvidar en el encargo.

### Encargo
cada estudiante debe tomar 2 de las 4 secciones distintas del sintetizador realizado en el proyecto 1, y crear un proyecto en KiCad por cada una, que contenga tanto el esquemático y la PCB de cada sección.

Proyecto 01:
secciones: clock generator y secuenciador

Partí haciendo el esquematico para luego ir todo el tema de placa, cambie el rv1 por un ldr.
![kikat-esquema](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/bc9f398607a320edcbe394e97a51998a5e994ce6/12-paulafuentesm/sesion-09a/imagenes/encargo/kikat-esquema.png)

Despues fue a la placa, para darme cuenta que no estaban todos los elementos, lo que paso fue: 

Problema: El chip CD4017 no aparecía en el diseño de la placa dentro del programa.

Solución: El componente no tenía una huella (footprint) asignada. Tras revisarlo, busqué y asigné la huella correspondiente, aunque el proceso tomó tiempo porque costó encontrar el encapsulado correcto: THT DIP/DIL PDIP de 16 pines, paso 2.54 mm y ancho 7.62 mm (300 mil).

Todos los elemento:
Se buscó una disposición ordenada en la que todos los terminales positivos de los LED quedaran orientados hacia arriba.
![kikat-orden](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/55860c6316c810912c818971315b913361f8f38c/12-paulafuentesm/sesion-09a/imagenes/encargo/kikat-orden.png)

Despues de tener todos los emelentos de la esquema, paso a colocar los cables segun las capas y diametros dispuestos en la clase, ya despues conectados todos los cables a los positivos, dejo libres los GND para colocar la zona rellan por esté.

![kikat-orden](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/55860c6316c810912c818971315b913361f8f38c/12-paulafuentesm/sesion-09a/imagenes/encargo/kikat-cables.png)

Para luego comprobar si habia algun error, aprete comprobar reglas de diseño y nose porque, no leia la placa aunque copiaba t pegaba el contorno, por lo que lo volvi a hacer 
![error2](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/55860c6316c810912c818971315b913361f8f38c/12-paulafuentesm/sesion-09a/imagenes/encargo/error2.png)

Solucionado: 

![placa-3d2](https://github.com/paulafuentesm/dis8644-2026-1-procesos-2/blob/2601efb6e92405a7efad3fc5ae9745003b322a21/12-paulafuentesm/sesion-09a/imagenes/encargo/placa-3d2.png)

Una vez realizado nuevamente el contorno, el programa reconoció correctamente la forma de la placa y no se detectaron más errores en el archivo, dejando la placa lista.

Preguntas:
+ Como buscar los elementos de chip u otros si es que no me salen con los nombres que ocupamos en clases? ya que no encontraba el chip 4017 y busque en chatgtp.

### Lectura: Hacia una filosofía de la fotografia 

#### Capitulo 1: La imagen 

**"Las imágenes son superficies significativas. En la mayoría de los casos, éstas significan algo 'exterior', y tienen la finalidad de hacer que ese 'algo' se vuelva imaginable para nosotros"**

+ Fución: las imágenes hacen que el mundo de las ideas se vuelva real para nosotro de una forma representativa, capturando la esencia del espacio y el tiempo
  
+ El significado de una imagen no se capta de manera lineal, sino que genera una dimensión de regreso eterno y produce símbolos connotativos ( fotogramas creo) abiertos a la interpretación.

+ las imágenes son mágicas: las imágenes erróneamente se ven como eventos congelados, sino que se crea  una ilusión respecto al evento transcurrido en la fotografía
+ el texto es la explicación de la imagen y descubrir a que se refiere el escena de la fotografía, se da un hecho de la que tiene que pasar en la foto por lo que no se esta abierto auna interpretación.
  
+ **el universo de la ciencia es un universo vacía, ya que no se deja nada a la interpretación de la persona, todo está dicho y concretado, por que si se ignora, está incorrecto, no existe la interpretación.** 

**"Se colocan en lugar del mundo a tal grado que el hombre vive en función de la imagen que el mismo ha producido"**

#### Destacado texto: 
**" Donde los textos ya no se imaginable, no hay nada que explicar y la historia cesa."**

+ la textolatria (adoración excesiva de los textos ) alcanzo el punto critico donde ya no existe la interpretacion ( magía o imaginacion) donde la imagen tenga una libre interpreteacion y donde todo esta mas definido, donde el ser humano ya no necesita pensar o analizar algo ( comparacion con el mundo actual ), segun yo, esto proboca que se cree un ser humano mas flojo donde todo necesita ser digerido rapido y explicito, donde mientras mas facil sea de digerir el texto ( tiktok o contenido basura) mas idiota se vulve el ser humano y mayor es su utilidad en el mundo capital ( hipotesis mia ). 






