## Intro

Me llamo Andrés soy un estudiante de matemáticas aplicadas y ciencias de datos en el ITAM. Paso todo mi tiempo diseñando y jugando con programas que produzcan resultados interesantes, tanto estéticos como experiencias interactivas. Trabajo principalmente con Unity y TouchDesigner. Debajo se encuentra mi portafolio que contiene los proyectos más relevantes que hecho en el ultimo año y las técnicas que he aprendido para poder implementarlos.


## Portafolio 
**Mandelbrot GLSL-TouchDesigner**

Este proyecto es una herramienta para explorar el famoso conjunto de mandelbrot. Posteriormente, convertí el fractal en audioreactivo. La implementación es relativamente simple, convertimos la textura a un espacio que va de [-1, 1] en "x" y igual en "y", dejando a cada pixel con un identificador en ese rango. Asignamos un valor ¨resultado¨ y en un loop se hace una operación al resultado que depende de la vuelta pasada. Dependiendo de que tanto  crezca "resultado", es como coloreamos el pixel. 

Está operación se hace cada frame para todos los pixeles, entonces para hacer los movimietnos del fractal, solamente había que desplazar, reducir o incrementar el rango de los identificadores. Es decir para ver más a la izquierda del fractal, debiamos hacer que los pixeles vayan de [-2,0] en "x" y en "y" permanecieran iguales. 

https://github.com/user-attachments/assets/45790cdb-8b24-425b-8f4a-bef6a2e42f66





<p>

  
## Pointcloud Experiments

Este año hice dos proyectos interesantes con, pointclouds, el primero:



**Spherical Gravity TouchDesiger GLSL**

Este proyecto nace de un video que habla sobre que es realmente la gravedad, que no es una fuerza como tal que jala a los objetos. Mas bien un campo gravitacional literalmente dobla el espacio. Las líneas blancas representan el espaico tridimensional en el que habitamos, son contraidas por el objeto en el centro, entre más se contraen más fuerza gravitacional tiene el objeto. 

https://github.com/user-attachments/assets/5176f8b3-8e50-479f-a63c-6b3ed25c5d67


Las líneas están hechas de 200,000 puntos en total aprox. Cada punto tiene una coordenada y usando un pixel shader que lee las coordenadas XYZ como colores RGB, se aplica la transformación. Dependiendo que tan lejos este el pixel del centro gravitaciónal es más notorio el efecto. En la video anterior se puede ver como se aumenta y decrementa la fuerza gravitacional. 


**Coordenadas polares**
Me pareció interesante que pasaría si además de aplicar gravedad también aplicaramos una transformación a coordenadas polares. Básicamente cualquier punto (x,y) lo podemos ver como un vector y sacar su tamaño y ángulo de inclinación nos daría sus coordenadas polares. 

Finalmente ajustamos los ángulos de nuestros nuevos puntos. El resultado ya no se apega a la realidad pero me gusto bastante.


https://github.com/user-attachments/assets/4e5555e4-b39c-4b27-b432-19360064908a



