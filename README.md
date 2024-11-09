
# Intro

Hola, me llamo Andrés, soy un estudiante en Ciudad de México de Matemáticas Aplicadas y Ciencias de Datos en el ITAM. Paso mi tiempo diseñando y jugando con programas que produzcan resultados interesantes. 

Principalmente me interesan los `displays interactivos`, ya sean:

`Videojuegos educativos`

`Estructuras interesantes`

`Realidad Aumentada`

Trabajo con Unity y TouchDesigner. Debajo se encuentra mi portafolio, contiene mis proyectos más relevantes y algunas técnicas que he aprendido para poder implementarlos.

Me puedes mandar un correo a **andressevilla81@gmail.com**

# Portafolio

## Meteorite 

Estoy `trabajando` en Meteorite `actualmente`:

Una `nave` viajando en el espacio a `gran velocidad` que debe evitar asteroides y naves enemigas.

**Meteorite3D**

![Meteorite3dClip](https://github.com/user-attachments/assets/ed9a4dc2-f446-4bbc-b045-c096f70cdfcb)

La `nueva` `versión es en 3D`, pero la idea nace de los juegos shoot 'em up de los 80-90's y  `la primera` es `una versión en 2D.`

**Meteorite2D**

![Meteorite2dClip](https://github.com/user-attachments/assets/e97e80de-63ea-46aa-be53-cf1baaf0f02a)

## Dive In

`Un juego inspirado por el buceo.`

Se trata de `aprender del océano` y de las especies que viven en él.

El jugador `explora un laberíntico arrecife` de corales en busca `de animales` que pueda conocer. Cada uno tiene `datos muy interesantes` que comparten con el jugador si los encuentra.

![DiveINlvl2clip](https://github.com/user-attachments/assets/25ed037c-8543-4767-864e-97dca579d2ad)

**¡No se te vaya a acabar el oxígeno!**

![DiveIN1](https://github.com/user-attachments/assets/edef0bae-5085-4f4d-a9eb-0eae193c81eb)

## GridSpace

**GridSpace Engine HLSL - UNITY**

[GridSpace](https://github.com/andressev/GridSpacee) es un motor de autómatas celulares.

Un `autómata celular` es cualquier `regla` que se le aplique individualmente a un grupo de píxeles, en intervalos de tiempo. Las reglas principalmente consisten en `preguntarle a un píxel sobre su entorno`: ¿cuántos píxeles están prendidos en un radio de n? Con la respuesta, puedes decirle al píxel que se apague, que se prenda, que no haga nada, etc.

El punto es que hay una `infinidad de reglas posibles`, una infinidad de entornos posibles. A cada una de estas acomodaciones posibles las llamaremos `estados`. Los estados por lo general son `bastante caóticos`, pero de vez en cuando se organizan para crear algo que asemeja a la vida celular.

El propósito de GridSpace es `compartir con sus usuarios un pedazo de este espacio infinito` y facilitar el viaje entre todos los estados. [Aquí](https://github.com/andressev/GridSpacee) se puede descargar GridSpace.

**Inicialmente el usuario crea un entorno-vecindario para efectuar las reglas.**

![GifNeighborhoods](https://github.com/user-attachments/assets/50d62360-fe90-4d12-9d1b-b9752f77f903)

**Luego escoge hasta 4 entornos/vecindarios.**

![GifNHpicker](https://github.com/user-attachments/assets/5dcbd464-9484-418f-a433-c6ba10b94331)

Después, el usuario, `usando los controles`, puede mutar las reglas para encontrar los estados más interesantes.

**Mutation mode**

![GridSpace Portafolio](https://github.com/user-attachments/assets/15eea6ea-17d4-42ae-805a-d90a68d3d044)

El usuario puede `viajar cómodamente` `mediante mutaciones de las células`. En todo GridSpace existen `10^308 estados posibles`; la cantidad de átomos en el universo son 10^80.

[Video de gameplay MutationMode](https://www.youtube.com/watch?v=BqFUAaOdQgY)

## Pointcloud Experiments

**Gravedad físicamente precisa TouchDesigner GLSL**

Este proyecto nace de intentar `representar precisamente la gravedad` en el espacio; no es una fuerza en realidad. Más bien, `un campo gravitacional literalmente dobla el espacio`.

Las líneas blancas representan el espacio tridimensional en el que habitamos; son contraídas por el objeto en el centro. `Se contraen` más `cuanto más cerca al centro` `o dependiendo de la cantidad de masa del centro`.

https://github.com/user-attachments/assets/5176f8b3-8e50-479f-a63c-6b3ed25c5d67

Las líneas están hechas de aproximadamente 200,000 puntos en total. Se aplica la transformación gradual a cada uno de los puntos que `replica el efecto que tiene la gravedad en la tela del espacio`.

**Spherical Gravity**

Si además de `transformar` para emular la gravedad, también aplicáramos una transformación a los `ángulos con respecto al origen`, obtenemos un resultado que ya no se apega a la realidad, pero es bonito.

https://github.com/user-attachments/assets/4e5555e4-b39c-4b27-b432-19360064908a

## Mandelbrot

**Mandelbrot 2D GLSL-TouchDesigner**

Este proyecto es una `herramienta para explorar` el famoso conjunto de `Mandelbrot`. Después, convertí el fractal en `audioreactivo.`

**Sound On**

https://github.com/user-attachments/assets/45790cdb-8b24-425b-8f4a-bef6a2e42f66

**Mandelbrot 3D Raymarched**

También aprendí un poco de `raymarching`, que es una técnica para proyectar y crear formas tridimensionales en un plano a través de funciones de distancia. `Encontré una función` para una `versión 3D de Mandelbrot` y, con TouchDesigner y algunos trucos de iluminación, este fue el resultado.

https://github.com/user-attachments/assets/5d88fa54-8d69-4e60-a4db-23ef1f518690
