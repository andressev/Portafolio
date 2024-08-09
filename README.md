
# Intro

Hola, me llamo Andrés, soy un estudiante de Matemáticas Aplicadas y Ciencias de Datos en el ITAM. Paso mi tiempo diseñando y jugando con programas que produzcan resultados interesantes, tanto estéticos como experiencias interactivas. Trabajo principalmente con Unity y TouchDesigner. Debajo se encuentra mi portafolio, que contiene los proyectos más relevantes que he hecho en el último año y las técnicas que he aprendido para poder implementarlos.

# Portafolio

## GridSpace

**GridSpace Engine HLSL - UNITY**

[GridSpace](https://github.com/andressev/GridSpacee) es el proyecto en el que llevo trabajando los últimos meses. Es un motor de autómatas celulares, un autómata celular es cualquier regla que se le aplique individualmente a un grupo de píxeles, en el caso de GridSpace: 1028x512 píxeles. Las reglas principalmente consisten en preguntarle a un píxel sobre su entorno, ¿cuántos píxeles están prendidos en un radio de n? Con la respuesta puedes decirle al píxel que se apague, que se prenda, que no haga nada, etc. 

El punto es que hay una infinidad de reglas posibles, una infinidad de entornos posibles. A cada una de estas acomodaciones posibles lo llamaremos estados. Los estados por lo general son bastante caóticos, pero de vez en cuando se organizan para crear algo que asemeja a la vida celular.

El motor está construido utilizando compute shaders y un sistema de buffers dinámicos, lo que permite procesar las reglas de los autómatas celulares de manera eficiente en el GPU. Esto facilita la exploración de un vasto espacio de estados posibles en tiempo real.

El propósito de GridSpace es compartir con sus usuarios un pedazo de este espacio infinito y facilitar el viaje entre todos los estados. [Aquí](https://github.com/andressev/GridSpacee) se puede descargar GridSpace.

**Inicialmente el usuario crea un entorno-vecindario para efectuar las reglas.**

![GifNeighborhoods](https://github.com/user-attachments/assets/50d62360-fe90-4d12-9d1b-b9752f77f903)

**Luego escoge hasta 4 entornos/vecindarios.**

![GifNHpicker](https://github.com/user-attachments/assets/4b6dffc1-a23e-48b7-85d1-b621b58c3c62)

Después, el usuario, usando los controles, puede mutar las reglas para encontrar los estados más interesantes.

**Mutation mode**

![GridSpace Portafolio](https://github.com/user-attachments/assets/15eea6ea-17d4-42ae-805a-d90a68d3d044)

En este modo, el usuario ya no necesita crear vecindarios, estos se generan y cambian automáticamente con las mutaciones. Cada uno de los estados está codificado en una secuencia de 32 enteros, por lo tanto en todo GridSpace existen 10^308 estados posibles; la cantidad de átomos en el universo son 10^80.

[Video de gameplay MutationMode](https://www.youtube.com/watch?v=BqFUAaOdQgY)

## Pointcloud Experiments

**Gravedad físicamente precisa TouchDesigner GLSL**

Este proyecto nace de un video que habla sobre qué es realmente la gravedad, que no es una fuerza como tal que jala a los objetos. Más bien, un campo gravitacional literalmente dobla el espacio. Las líneas blancas representan el espacio tridimensional en el que habitamos, son contraídas por el objeto en el centro; entre más se contraen, más fuerza gravitacional tiene el objeto.

https://github.com/user-attachments/assets/5176f8b3-8e50-479f-a63c-6b3ed25c5d67

Las líneas están hechas de 200,000 puntos en total aproximadamente. Cada punto tiene una coordenada y, usando un pixel shader que lee las coordenadas XYZ como colores RGB, se aplica la transformación. Dependiendo de qué tan lejos esté el píxel del centro gravitacional, es más notorio el efecto. En el video anterior se puede ver cómo se aumenta y decrementa la fuerza gravitacional.

**Spherical Gravity**

Me pareció interesante qué pasaría si, además de aplicar gravedad, también aplicáramos una transformación a sus coordenadas polares. Básicamente, cualquier punto (x,y) lo podemos ver como un vector, y sacar su tamaño y ángulo de inclinación nos daría sus coordenadas polares.

Finalmente, ajustamos los ángulos de nuestros nuevos puntos. El resultado ya no se apega a la realidad, pero me gustó bastante.

https://github.com/user-attachments/assets/4e5555e4-b39c-4b27-b432-19360064908a

## Mandelbrot

**Mandelbrot 2D GLSL-TouchDesigner**

Este proyecto es una herramienta para explorar el famoso conjunto de Mandelbrot. Posteriormente, convertí el fractal en audioreactivo. La implementación es relativamente simple: convertimos la textura a un espacio que va de [-1, 1] en "x" e igual en "y", dejando a cada píxel con un identificador en ese rango. Asignamos un valor "resultado" y, en un loop, se hace una operación al resultado que depende de la vuelta pasada. Dependiendo de qué tanto crezca "resultado", es como coloreamos el píxel.

Esta operación se hace cada frame para todos los píxeles, entonces, para hacer los movimientos del fractal, solamente había que desplazar, reducir o incrementar el rango de los identificadores. Es decir, para ver más a la izquierda del fractal, debíamos hacer que los píxeles vayan de [-2,0] en "x" y en "y" permanecieran iguales.

https://github.com/user-attachments/assets/45790cdb-8b24-425b-8f4a-bef6a2e42f66

**Mandelbrot 3D Raymarched**

Después de unos meses, aprendí un poco de raymarching, que es una técnica para proyectar y crear formas tridimensionales en un plano a través de funciones de distancia. Encontré una función para una versión 3D de Mandelbrot y, con TouchDesigner y algunos trucos de iluminación, este fue el resultado.

https://github.com/user-attachments/assets/5d88fa54-8d69-4e60-a4db-23ef1f518690
