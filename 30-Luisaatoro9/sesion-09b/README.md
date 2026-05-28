# sesion-09b 15 de mayo

Componentes Propios y el Proyecto de Filtros 

### Correcciones: Lo que no hay que hacer

En la clase de hoy repasamos los errores típicos que nos pasaron a todos. Lo más importante, es que si cambio algo en el esquema (como el valor de una resistencia), la placa no se actualiza sola. Tengo que darle a "Actualizar placa desde esquema" o voy a terminar mandando a fabricar algo que no sirve.

También vimos lo de las islas de cobre. Cuando relleno con GND, a veces quedan pedazos de cobre sueltos por ahí. Si tienen una X, es que están mal porque no pueden disipar calor. Tienen que tener al menos 3 conexiones para estar bien.

Esto fue lo más pro de la clase. A veces el componente que necesitas no existe o las patitas están en otro orden.

* **Editor de Símbolos:** Aprendí que NUNCA hay que editar el original porque arruinas todos mis proyectos.
* **Hacer un Fork:** Básicamente es copiar un símbolo a mi propia biblioteca (.kicad_sym) y ahí sí, cambiarle lo que quiera con la tecla E o mover pines con la tecla M.
* **Tip:** Si veo un asterisco (*) arriba, tengo que guardar los cambios.

### Mi proyecto 2: Grupo de Filtros
<img width="656" height="532" alt="image" src="https://github.com/user-attachments/assets/e137b730-a1ff-42b8-b38c-fee308fca614" />

### Libro Hacia una filosofía de la fotografía, continuación de la lectura...

Cap 2: El Aparato y la Caja Negra (KiCad vs. Realidad)
<p>
 Al leer sobre el 'Aparato', no pude evitar pensar en el KiCad. Flusser dice que un aparato es una 'caja negra' porque usamos su programa sin saber exactamente qué pasa en el código interno. En el ramo, cuando pasamos del esquema al PCB y lo vemos en 3D, estamos usando un aparato que ya tiene 'pre-programado' cómo debe verse una placa. El riesgo, como dice Flusser, es quedarnos solo en la superficie. Por eso, aprender a leer los circuitos y entender qué hace cada componente en la protoboard es como intentar abrir esa caja negra para no ser solo usuarios que aprietan botones, sino diseñadores que entienden la lógica interna.
</p>

Cap 3: El Gesto de Fotografiar (Cazar el diseño del Filtro)
<p>
  Flusser habla del 'gesto' como una cacería de posibilidades dentro de un programa. Esto me pasó tal cual eligiendo las propuestas para el proyecto de filtros. No es que inventé la electricidad, sino que 'cacé' las mejores combinaciones de resistencias y condensadores dentro de lo que la teoría de filtros permite. Mi 'gesto' en el KiCad, moviendo componentes y ruteando pistas, es exactamente esa búsqueda que describe Flusser, elegir entre las infinitas opciones que el programa me da para que el filtro funcione y se pueda mandar a fabricar.
</p>

Cap 4: La Fotografía (La placa 3D como Imagen Técnica)
<p>
  Este capítulo dice que las imágenes técnicas son conceptos convertidos en imágenes. La visualización 3D de nuestra placa de filtros no es la placa real todavía, es una 'imagen técnica' basada en las leyes de la física y la electrónica que el software traduce. Lo que Flusser advierte es que no debemos confundir esa imagen con la realidad. Por eso es tan importante armar el circuito en la protoboard, ahí es donde la teoría (el concepto) se choca con la materia real y vemos si el filtro de verdad filtra o si solo se veía bonito en el render del KiCad.
</p>

Cap 5: La Distribución (De la pantalla a la fabricación)
<p>
  Flusser explica que en la era de los aparatos lo que importa es la información, no la materia, porque la info se puede reproducir mil veces. Esto lo veo directo en nuestro flujo de trabajo, una vez que terminamos el diseño de los filtros en KiCad, lo que mandamos a la fábrica no es una placa física, es un archivo (información). La fábrica es el aparato que 'distribuye' nuestro diseño en serie. Como dice Flusser, mi rol cambia, ya no soy un artesano que lija cobre, soy un programador de hardware que genera información para que una máquina la ejecute.
</p>

Conclusión Personal: **La Libertad y la Rebeldía de Diseñar**

Lo que más me marcó de esta lectura fue el concepto de 'funcionario'. Flusser advierte que, si solo seguimos las reglas del aparato, dejamos de ser creadores. Al venir del mundo de la ingeniería, sentía que a veces te enseñan a seguir patrones, fórmulas dadas, recopilar datos y ver problemáticas de forma estructurada. Pero al entrar en Diseño, entendí que esta carrera te entrega libertad, aunque es una libertad que hay que ganar.

Siento que para diseñar de verdad hace falta una cuota de rebeldía interna. Si no tienes ese cuestionamiento mental o esa madurez para ver más allá, terminas simplemente cumpliendo con lo que el sistema te pide. La originalidad nace de esa rebeldía de querer forzar al aparato (ya sea el KiCad o la vida misma) a que haga algo más, algo que salió de tu cabeza y no de un manual. Mi meta con este proyecto de filtros es esa, usar la técnica no para repetir patrones, sino para demostrar que lo que uno crea en la mente puede ser real si no dejas que el 'programa' limite tu visión. Es, finalmente, dejar de ser funcionaria para ser una artesana con pensamiento propio.

 **"No te fijes solo en los árboles, fíjate en quién plantó el bosque".**
 
---
Glosario rápido de lo que aprendí
1. DRC (Design Rule Checking): Es el "policía" del programa que me dice si las pistas están muy juntas o si algo va a explotar.
2. Gerber: Es el formato final. Es como el "PDF" de las placas, se lo mando a la fábrica y listo.

### Referencias

- [KiCad — editor de símbolos](https://docs.kicad.org/master/en/eeschema/eeschema.html#symbol-editor)
- [Tipos de interruptores — push vs switch](https://www.electronics-tutorials.ws/io/io_1.html)
- [3PDT switch — cómo funciona en pedales de guitarra](https://www.electrosmash.com/boss-ds1-analysis)
- [Huellas DIP en KiCad](https://docs.kicad.org/master/en/pcbnew/pcbnew.html)
