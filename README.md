# Mi primer docker
## Daniel Sobrino

Tras comprobar que tengo instalado docker gracias al comando ```docker ps```, ejecuto el ```build.sh```. Esta es la salida por consola:

![1-buildsh](https://user-images.githubusercontent.com/91564560/161798552-60edf1b2-8b80-4a7c-819f-29dd75520310.png)

Una vez creado el contenedor a partir del archivo Dockerfile, lanzo el contenedor en modo debug con ```debug.sh```.

![2-debugsh-fail](https://user-images.githubusercontent.com/91564560/161798822-f1dca992-5b79-46a5-9029-9c3f0c97e1fb.png)

![3-debugsh-5counter](https://user-images.githubusercontent.com/91564560/161798837-a1837880-c6fe-4ac2-b087-7eeb33a3555c.png)

He podido comprobar que el contador de visitas aumenta. Sin embargo, para que éste sea persistente, tendré que ejecutar el ```persist.sh```, que crea un volumen con el nombre del directorio del huésped, permitiendo guardar la información entre sesiones. Esta es la salida por consola:

![4-persist](https://user-images.githubusercontent.com/91564560/161799331-21146945-4ef3-490d-89cf-34312059580f.png)

Y aquí he realizado varias pruebas:

![prueba_datos_persistentes](https://user-images.githubusercontent.com/91564560/161799392-bd8cab0d-4ade-47b3-b210-b9fc7b0edc20.png)
