## Intro

Me llamo Andrés soy un estudiante de matemáticas aplicadas y ciencias de datos en el ITAM. Paso todo mi tiempo diseñando y jugando con programas que produzcan resultados interesantes, tanto estéticos como experiencias interactivas. Trabajo principalmente con Unity y TouchDesigner. Debajo se encuentra mi portafolio que contiene los proyectos más relevantes que hecho en el ultimo año y las técnicas que he aprendido para poder implementarlos.


## Portafolio 

## GridSpace 

**GridSpace Engine HLSL - UNITY** 

[GridSpace](https://github.com/andressev/GridSpacee) es el proyecto en que ue llevo trabajando los ultimos meses.  Es un motor de automatas celulares, un automata celular es cualquier regla que se le aplique individualmente a un grupo de pixeles, en el caso de GridSpace 1028x512 pixeles. Las reglas principalmente consisten en preguntarle a un pixel sobre su entorno, cuántos pixeles estan prendiddos en un radio de n? Con la respuesta puedes decirle al pixel que se apague, que se prende, que no haga nada, etc. El punto es que hay una infinidad de reglas posibles, una infinidad de entornos posibles. A cada una de estás acomodaciones posibles lo llamaremos estados. 

El proposito de GridSpace es compartir con sus usuarios un pedazo de este espacio infinito y facilitar el viaje entre todos los estados. [Aqui](https://github.com/andressev/GridSpacee) se puede descargar GridSpace. 

**Inicialmente el usuario crea un entorno-vecindario para efectuar las reglas.** 

![GifNeighbrohoods](https://github.com/user-attachments/assets/50d62360-fe90-4d12-9d1b-b9752f77f903)

**Luego escoge hasta 4 entornos/vecindarios.**

![GifNHpicker](https://github.com/user-attachments/assets/4b6dffc1-a23e-48b7-85d1-b621b58c3c62)

Después el usuario usando los controles puede mutar las reglas para encontrar los estados más interesantes.

**Mutation mode** 

![GridSPace Portafolio](https://github.com/user-attachments/assets/15eea6ea-17d4-42ae-805a-d90a68d3d044)


En este modo el usuario ya no necesita crear vecindarios, estos se generan y cambian automaticamente con las mutaciones. Cada uno de los estados esta codificado en una sequencia de 32 enteros. En todo gridspace existen 10^308 estados posibles, la cantidad de átomos en el universo son 10^80. 

[Video de gameplay MutationMode](https://www.youtube.com/watch?v=BqFUAaOdQgY)
  
## Pointcloud Experiments


**Gravedad Fisicamente precisa TouchDesiger GLSL**

Este proyecto nace de un video que habla sobre que es realmente la gravedad, que no es una fuerza como tal que jala a los objetos. Mas bien un campo gravitacional literalmente dobla el espacio. Las líneas blancas representan el espaico tridimensional en el que habitamos, son contraidas por el objeto en el centro, entre más se contraen más fuerza gravitacional tiene el objeto. 





https://github.com/user-attachments/assets/5176f8b3-8e50-479f-a63c-6b3ed25c5d67


Las líneas están hechas de 200,000 puntos en total aprox. Cada punto tiene una coordenada y usando un pixel shader que lee las coordenadas XYZ como colores RGB, se aplica la transformación. Dependiendo que tan lejos este el pixel del centro gravitaciónal es más notorio el efecto. En la video anterior se puede ver como se aumenta y decrementa la fuerza gravitacional. 




**Spherical Gravity**
Me pareció interesante que pasaría si además de aplicar gravedad también aplicaramos una transformación a sus coordenadas polares. Básicamente cualquier punto (x,y) lo podemos ver como un vector y sacar su tamaño y ángulo de inclinación nos daría sus coordenadas polares. 

Finalmente ajustamos los ángulos de nuestros nuevos puntos. El resultado ya no se apega a la realidad pero me gusto bastante.


https://github.com/user-attachments/assets/4e5555e4-b39c-4b27-b432-19360064908a


## Mandelbrot
**Mandelbrot 2D GLSL-TouchDesigner**

Este proyecto es una herramienta para explorar el famoso conjunto de mandelbrot. Posteriormente, convertí el fractal en audioreactivo. La implementación es relativamente simple, convertimos la textura a un espacio que va de [-1, 1] en "x" y igual en "y", dejando a cada pixel con un identificador en ese rango. Asignamos un valor ¨resultado¨ y en un loop se hace una operación al resultado que depende de la vuelta pasada. Dependiendo de que tanto  crezca "resultado", es como coloreamos el pixel. 

Está operación se hace cada frame para todos los pixeles, entonces para hacer los movimietnos del fractal, solamente había que desplazar, reducir o incrementar el rango de los identificadores. Es decir para ver más a la izquierda del fractal, debiamos hacer que los pixeles vayan de [-2,0] en "x" y en "y" permanecieran iguales. 

https://github.com/user-attachments/assets/45790cdb-8b24-425b-8f4a-bef6a2e42f66


**Mandelbrot 3D Raymarched**

Después de unos meses aprendí un poco de raymarching, que es una técnica para proyectar  y crear formas tridimensionales en un plano a través de funciones de distancia. Encontré una función para una versión 3D de mandelbrot y con touchdesigner y algunos trucos de iluminación este fue el resultado. 



https://github.com/user-attachments/assets/5d88fa54-8d69-4e60-a4db-23ef1f518690





