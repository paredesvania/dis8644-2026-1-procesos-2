# sesion-11a

- ## me enferme!! y no pude asistir presencialmente :(

  - texto flusser 6/7
    - la distribución de la fotografía
      - la fotografía es informacíon que está anclada a algo material
      - las imagenes se distribuyen y clasifican en 3 categorias
        - Documentación cientifica
        - Politica
        - Artistica
          - (yo opino que finalmente todas las categorías se interconectan, el arte es politico al igual que la ciencia y viceversa, pero entiendo porqué hace la distinción)
      - hay una influencia mutua entre las fotografías y las categorias mencionadas anteriormente
      - también habla de que "la imagen subordina al texto"
        - ganando en que el ser común se guía más por imagenes idealizadas de algo, que por el objeto mismo
          - sin pensamiento critico de la imagen
            - de donde es la foto?
            - quién la saco?
            - cual fue la intención?
            - cual es el contexto?
            - que **no** se ven en la imagen?
           
- ## avances piezo
  - con mi grupo nos juntamos el lunes 25 a trabajar en las proto
- ![con grupo 1](./imagenes/piezo-1.jpg)
- ![con grupo 2](./imagenes/piezo-2.jpg)
    - revisamos el problema del reset con el 4017 mencionado en la sesion anteriór
      - al hacer el esquema del piezo 1 en la protoboard notamos que la señal del piezo llegaba al 555
      - ![intento 1](./imagenes/piezo-1.gif)
        - la luz conectada al 555 se prende al pegarle al piezo
    - volvimos a ver las conexiónes y ahora al pegarle al piezo, reaccionaban 1 de las 2 luces en el 4017
      - ![intento 2](./imagenes/piezo-2.gif)
        - la otra se mantenía prendida
    - el circuito era muy poco estable, de vez en cuando se prendian las luces y no siempre reaccionaban al piezo
      - en este intento una de las 2 luces en el 4017 se prendían y alternaban al tocar el piezo
      - ![intento 3](./imagenes/piezo-3.gif)
        - algo importante, aquí el pin de RST esta "conectado" al aire, con un final del cable en el pin 15 y el otro final sin conectar
          - ![RST aire](./imagenes/rst-suelto.jpg)
    - aquí logramos tener una mejor respuesta en cuanto al RST
      - lo conectamos con un capacitor 104 a tierra para que sea más estable
        - ![intento 4](./imagenes/piezo-4.gif)
    - finalmente llegamos a la versión más estable del v01
      - añadimos un segundo piezo para simular mejor la idea del Taiko como juego de tambor con 2 baquetas
      - ![intento 5-1](./imagenes/funcionandoish.gif)
      - ![intento 5-2](./imagenes/cerca-funcionandoish.gif)
     
  - ### sin musica detallada porque me siento mal y tengo que dormir
    - pero estos son 3 albumes que escuché haciendo el trabajo

      - **Quadeca - Vanisher, Horizon Scraper**
        - https://music.youtube.com/playlist?list=OLAK5uy_mcNa_NXSwYITwnILZHoQHPxRFy_LSHiSA&si=i1fxXl7cewBfsam2
          -  (no está en bandcamp)
      - **Oidopuaa Vladimir Oiun - Divine Music from Jail**
        - https://ebalunga.bandcamp.com/album/divine-music-from-jail
      - **Jockstrap - I Love You Jennifer B**
        - https://jockstrapmusic.bandcamp.com/album/i-love-you-jennifer-b
