## Instrucciones
1.comprobamos que la maquina tenga instalados docker y git, si no los tiene se ejecutaran los siguienetes comandos y si pregunta en algún punto por una confirmacion seleccionamos yes(y) ;

- sudo apt update

- sudo apt install git

- sudo apt install docker.io

2.Despues ingresamos a la carpeta /proyecto-telematica y ejecutamos el siguiente comando siempre y cuando el puerto 80 no este en uso:

- sudo docker build -t servermap:v01 .

3.para finalizar ejecutamos el siguente comando:
- sudo docker run -d -p 80:80 servermap:v01

4.para comprovar que el servicio funcione simplemente pon la ip de la maquina en cualquier navegador, al estar funcionando por el puerto 80 que es el que viene por defecto pero tambien puedes especificar el puerto y funcionaría igual.
