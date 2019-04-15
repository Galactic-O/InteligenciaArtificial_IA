# Prácticas de la asignatura Inteligencia Artificial #
Prácticas de la asignatura Inteligencia Artificial del grado en Ingeniería Informática (UGR). Consisten en 3 prácticas diferentes que están divididas por niveles, cada uno realizando una función específica dentro de cada práctica.

## Práctica 1: Agente Conversacional ##

Bot conversacional usando el lenguaje AIML 2.0. He desarrollado 3 niveles de los 4 propuestos.

- **Nivel 0:** Contesta un total de 18 preguntas frecuentes que puedan aparecer en una entrevista de trabajo.
- **Nivel 1:** Introducción de contenidos en una plataforma de vídeo. Permite:
   + Incluir un nuevo capítulo en una temporada de una serie.
   + Incluir el primer capítulo de una nueva temporada en una serie.
   + Incluir una nueva serie en una de las plataformas.
- **Nivel 2:** Consultas sobre el contenido en una plataforma de vídeo. Permite:
   + Indicar los idiomas y subtítulos en los que se puede visionar una serie. Esto incluye preguntar si la serie está en un idioma concreto.
   + Responder al número de idiomas, subtítulos o capítulos totales o de una temporada que tiene una serie en concreto.
   + Indicar el número de temporadas que tiene la serie.
   + Decir el nombre de un capítulo concreto de una temporada de una serie.
   + Indicar la duración en minutos de un capítulo concreto de una serie.

Para iniciar el bot hay que ejecutar el archivo *run.sh*.

## Práctica 2: Agentes Reactivos/Deliberativos (Los extraños mundos de Belkan)

Los extraños mundos de Belkan es un simulador desarrollado por los profesores de la asignatura, a partir de la versión inicial del profesor Tsung-Che Chiang de la NTNU (Norwegian University of Science and Technology, Trondheim).

Se desarrolla sobre un un mapa cuadrado bidimensional discreto que contiene como máximo 100 filas y 100 columnas. El mapa representa los accidentes geográficos de la superficie de parte de un planeta semejante a la Tierra. Estos accidentes geográficos tendrán un coste mayor o menor de instantes de tiempo, lo que hará que el personaje tarde más tiempo en pasar por uno de estos lugares. Sus elementos son considerados inmutables, es decir, el mapa no cambia durante el desarrollo del juego.

El objetivo de esta práctica es dotar de un comportamiento inteligente al personaje usando un agente reactivo/deliberativo para definir las habilidades que le permitan alcanzar una meta concreta dentro del juego según el nivel seleccionado:

- **Nivel 1:** Agente deliberativo básico que conoce por completo el mapa y no hay aldeanos en este (los aldeanos son el único elemento móvil del juego). El agente creará y llevará a cabo un plan que esquivará los muros y evitará caerse por los precipicios (límites del mapa) para así llegar al destino usando tres tipos de algoritmos de búsqueda:
   + Búsqueda en profundidad.
   + Búsqueda en anchura.
   + Búsqueda de costo uniforme.

El programa se inicia mediante el ejecutable *Belkan* (siendo *BelkanSG* una versión que funciona solo por terminal sin interfaz gráfica). Entonces se debe elegir uno de los niveles descritos y el mapa en el que se resolverá el problema. Para elegir una meta dentro del mapa sólo hace falta hacer click sobre el lugar en el mapa, y presionar el botón de "ejecución" para que el personaje vaya hacia ese lugar.
