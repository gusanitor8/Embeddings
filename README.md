## Laboratorio 8 - Embeddings

### Parte Teorica
1. El constructor del modelo Word2Vec acepta dos parámetros importantes:
    a. vector_size
    b. window

Describa la función que cumple cada uno de estos parámetros dentro del
algoritmo y disctua sobre las consecuencias de utilizar valores muy altos
o muy bajos para cada uno de estos parámetros. Indique en qué
situaciones podría ser apropiado ajustar de determinada manera (alto o
bajo) estos valores o si, en ciertos casos, nunca es recomendable hacerlo.   
---
  

El parámetro vector_size define la dimensionalidad de los embeddings generados, donde valores altos capturan más características semánticas pero aumentan el costo computacional y riesgo de sobreajuste, mientras valores bajos pueden simplificar pero perder información. window determina el número de palabras alrededor de una palabra objetivo que el modelo considerará como contexto; un valor alto abarca un contexto más amplio, útil en textos largos, mientras que uno bajo captura relaciones locales, más adecuado para textos cortos. Ajustar estos valores depende del tamaño del corpus: en textos grandes y diversos, valores más altos pueden ser útiles, mientras que en textos pequeños o específicos se prefieren valores bajos.