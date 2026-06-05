# Clase 12a — Decisión del filtro final

**Tema:** filtros, descarte del Sallen-Key y elección de un filtro pasivo de bajos y agudos  
**Trabajo de clase:** definición del tipo de filtro para el proyecto

---

## Resumen de la clase

En esta clase seguimos trabajando en la parte de los filtros para el proyecto. La idea era continuar armando y definiendo qué tipo de filtro íbamos a usar, tomando en cuenta lo que habíamos investigado en las clases anteriores sobre filtros activos, amplificadores operacionales y Sallen-Key.

Al principio todavía estábamos considerando usar el filtro **Sallen-Key**, porque era una opción interesante para hacer filtros activos de paso bajo o paso alto. Sin embargo, durante la clase se conversó que podía no ser la mejor opción para nuestro proyecto, principalmente porque trabajaba con frecuencias que podían no ser compatibles con los trabajos de los demás compañeros.

Por eso, se empezó a debatir qué tipo de filtro convenía más usar. La idea era encontrar una opción que fuera más simple, más compatible y más fácil de adaptar al proyecto general.

Finalmente, se decidió usar un filtro tipo **passive bass and treble**, es decir, un filtro pasivo para bajos y agudos.

---

## Por qué se descartó el Sallen-Key

El filtro **Sallen-Key** fue descartado porque, aunque era una buena opción técnica, podía complicar la integración con los otros proyectos.

El problema principal era que este filtro podía trabajar con rangos de frecuencia distintos a los que necesitábamos o a los que estaban usando otros compañeros. Esto hacía que no fuera tan conveniente seguir avanzando con esa opción.

Además, el Sallen-Key requiere un amplificador operacional, como el **LM324** o el **LM358**, y también necesita alimentación. Eso hacía que el circuito fuera más complejo para lo que necesitábamos en esta etapa.

En resumen, el Sallen-Key no era una mala opción, pero sí podía ser más difícil de adaptar al proyecto grupal.

---

## Debate sobre qué filtro usar

Durante la clase estuvimos revisando qué tipo de filtro podía funcionar mejor. La idea no era solamente elegir un circuito porque sí, sino pensar en algo que tuviera sentido dentro del proyecto completo.

Se consideraron principalmente estas cosas:

- Que el filtro fuera simple de armar.
- Que no dependiera tanto de un circuito integrado.
- Que no necesitara alimentación extra.
- Que pudiera adaptarse mejor a los trabajos de los demás.
- Que permitiera controlar bajos y agudos.
- Que fuera más fácil de probar y modificar.

Después de conversar estas opciones, la decisión fue avanzar con un filtro pasivo.

---

## Filtro elegido: Passive Bass and Treble

El filtro elegido fue un **passive bass and treble**, que funciona como un control pasivo de bajos y agudos.

Este tipo de filtro permite modificar la señal sin usar un circuito integrado. Esto lo hace más simple, porque no necesita un amplificador operacional ni alimentación externa.

```text
Passive bass and treble = filtro pasivo de bajos y agudos
```

La idea es poder controlar ciertas partes del sonido usando componentes pasivos como:

- resistencias;
- capacitores;
- potenciómetros.

Esto permite modificar el comportamiento de la señal sin tener que depender de chips como el LM324 o el LM358.

---

## Diferencia entre filtro activo y filtro pasivo

| Tipo de filtro | Características |
|---|---|
| Filtro activo | Usa amplificador operacional y necesita alimentación. |
| Filtro pasivo | Usa resistencias, capacitores y potenciómetros, sin alimentación extra. |

En nuestro caso, el filtro pasivo tenía más sentido porque era más simple y podía integrarse mejor con el resto del proyecto.

---

## Ventajas del filtro pasivo

Las principales ventajas del filtro pasivo fueron:

- No necesita circuito integrado.
- No requiere alimentación.
- Es más fácil de armar y probar.
- Usa menos componentes.
- Es más simple de adaptar.
- Puede controlar bajos y agudos.
- Reduce la complejidad del circuito general.

Esto fue importante porque veníamos de revisar opciones más complejas, como el Sallen-Key, y necesitábamos una solución más directa.

---

## Lo que se buscaba lograr

La idea del filtro era poder trabajar con el sonido y modificar ciertas frecuencias.

En simple:

```text
Bajos  → frecuencias graves
Agudos → frecuencias altas
```

Con el filtro pasivo de bajos y agudos, se puede ajustar qué parte de la señal se quiere destacar o reducir.

Esto puede servir para darle más control al sonido final del proyecto, sin tener que agregar demasiada complejidad electrónica.

---

## Componentes considerados

Para este tipo de filtro se podrían usar principalmente componentes pasivos:

| Componente | Función dentro del filtro |
|---|---|
| Resistencia | Ayuda a limitar o dividir la señal. |
| Capacitor | Permite filtrar ciertas frecuencias. |
| Potenciómetro | Permite ajustar manualmente bajos o agudos. |

A diferencia del Sallen-Key, este filtro no necesita un operacional como el LM324 o el LM358.

---

## Comparación entre Sallen-Key y Passive Bass and Treble

| Característica | Sallen-Key | Passive Bass and Treble |
|---|---|---|
| Tipo de filtro | Activo | Pasivo |
| Usa amplificador operacional | Sí | No |
| Necesita alimentación | Sí | No |
| Complejidad | Mayor | Menor |
| Compatibilidad con otros proyectos | Podía complicarse | Más fácil de adaptar |
| Control de frecuencias | Más técnico | Más directo |
| Decisión final | Descartado | Elegido |

---

## Ideas importantes que me quedaron

- El filtro Sallen-Key era interesante, pero no era lo más conveniente para este proyecto.
- La compatibilidad con los trabajos de los demás compañeros era importante.
- Un filtro más complejo no siempre es la mejor opción.
- El filtro pasivo de bajos y agudos es más simple y práctico.
- Al no usar integrado ni alimentación, se reduce la dificultad del circuito.
- Los filtros pasivos pueden ser una buena opción cuando se busca algo más directo.
- La decisión del filtro también depende del contexto del proyecto, no solo de la teoría.

---

## Reflexión personal

Esta clase sirvió para aterrizar mejor el proyecto. Al principio parecía que lo más lógico era seguir con el Sallen-Key porque ya lo habíamos investigado, pero después quedó claro que no siempre la opción más completa es la más útil.

El Sallen-Key podía funcionar bien como filtro activo, pero también agregaba más problemas: necesitaba alimentación, usaba un operacional y podía trabajar con frecuencias que no calzaban tan bien con los proyectos de los demás.

Por eso me pareció buena la decisión de usar un filtro pasivo de bajos y agudos. Es una solución más simple, pero también más fácil de adaptar. Además, permite concentrarse en cómo se comporta el sonido sin complicar demasiado el circuito.

---

## Conclusión

En la clase 12a se decidió descartar el filtro Sallen-Key y avanzar con un filtro **passive bass and treble**. Esta decisión se tomó porque el Sallen-Key podía generar problemas de compatibilidad con las frecuencias de otros proyectos y además requería más componentes, alimentación y circuitos integrados.

El filtro pasivo elegido permite controlar bajos y agudos de una forma más simple, sin usar amplificadores operacionales ni alimentación externa. Esto lo hace más práctico para seguir avanzando en el proyecto.

El siguiente paso sería probar el circuito pasivo, revisar cómo responde con la señal real y ajustar los valores de resistencias, capacitores o potenciómetros según el resultado que se quiera lograr.
