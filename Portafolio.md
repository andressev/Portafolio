# Intro

Me llamo Andrés soy un estudiante de matemáticas aplicadas y ciencias de datos en el ITAM. Paso todo mi tiempo diseñando y jugando con programas que produzcan resultados interesantes, tanto estéticos como experiencias interactivas. Trabajo principalmente con unity y touchdesigner. Debajo se encuentra mi portafolio que contiene los proyectos más relevantes que hecho en el ultimo año y las técnicas que he aprendido para poder implementarlos.


# Portafolio 

El primer proyecto que hice con GLSL en touch designer es una herramienta para explorar el famoso conjunto de mandelbrot. Posteriormente, convertí el fractal en audioreactivo. La implementación es relativamente simple, convertimos la textura a un espacio que va de [-1, 1] en "x" y igual en "y", dejando a cada pixel con un identificador en ese rango. Asignamos un valor ¨resultado¨ y en un loop se hace una operación al resultado que depende de la vuelta pasada. Dependiendo de que tanto  crezca "resultado", es como coloreamos el pixel. 

Está operación se hace cada frame para todos los pixeles, entonces para hacer los movimietnos del fractal, solamente había que desplazar, recudir o incrementar el rango de los identificadores. Es decir para ver más a la izquierda del fractal, debiamos hacer que los pixeles vayan de [-2,0] en "x" y en "y" permanecieran iguales. 

Finalmente para implementar la reactividad al sonido, los colores 


<iframe width="560" height="315" src="https://www.youtube.com/embed/ScF4T-9ZkrM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

