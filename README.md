## Intro

Me llamo Andrés soy un estudiante de matemáticas aplicadas y ciencias de datos en el ITAM. Paso todo mi tiempo diseñando y jugando con programas que produzcan resultados interesantes, tanto estéticos como experiencias interactivas. Trabajo principalmente con unity y touchdesigner. Debajo se encuentra mi portafolio que contiene los proyectos más relevantes que hecho en el ultimo año y las técnicas que he aprendido para poder implementarlos.


## Portafolio 
**Mandelbrot GLSL-TouchDesigner**

Este proyecto es una herramienta para explorar el famoso conjunto de mandelbrot. Posteriormente, convertí el fractal en audioreactivo. La implementación es relativamente simple, convertimos la textura a un espacio que va de [-1, 1] en "x" y igual en "y", dejando a cada pixel con un identificador en ese rango. Asignamos un valor ¨resultado¨ y en un loop se hace una operación al resultado que depende de la vuelta pasada. Dependiendo de que tanto  crezca "resultado", es como coloreamos el pixel. 

Está operación se hace cada frame para todos los pixeles, entonces para hacer los movimietnos del fractal, solamente había que desplazar, reducir o incrementar el rango de los identificadores. Es decir para ver más a la izquierda del fractal, debiamos hacer que los pixeles vayan de [-2,0] en "x" y en "y" permanecieran iguales. 

https://github.com/user-attachments/assets/45790cdb-8b24-425b-8f4a-bef6a2e42f66





<p>

  
## Pointcloud Experiments

Este año hice dos proyectos interesantes con, pointclouds, el primero:



**Spherical Gravity TouchDesiger GLSL**

400,000 puntos iniciales, se pueden aplicar 2 tipos de movimientos. El primero incrementar la gravedad y mover el centro de gravedad. 


https://github.com/user-attachments/assets/5176f8b3-8e50-479f-a63c-6b3ed25c5d67



