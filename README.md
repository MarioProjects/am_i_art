# Am I Art?

En el siguiente repositorio probamos una idea sencilla pero que puede llamar la atención: la búsqueda de parecidos entre caras dadas y caras en obras de arte.

Para ello necesitaremos lo siguiente:
  - Un [extractor de caras](https://github.com/ageitgey/face_recognition).
  - Una base de datos de obras de arte. Como [esta](https://www.kaggle.com/ikarus777/best-artworks-of-all-time).
  - Una red para crear los embeddings de las caras preentrenado. ¡[Aquí](https://github.com/timesler/facenet-pytorch) hay uno!
  
Con esto procederemos de la siguiente forma:
 
  1. Extraer las imagenes de la base de datos de obras de arte que contengan caras. Además almacenaremos tanto la posicion de la cara como su embedding. 
  2. Probar el funcionamiento con un test de búsqueda con una imagen con una cara cualquiera.
  3. Encapsularlo todo en una aplicación y permitir subir una imagen de donde se extraeran las caras y se buscaran las mas proximas.
  4. Mostrar el resultado de forma visual, imagen subida, imagen del cuadro, y poner cara junto cara parecida. También incluir información del artista. 