# Ejemplo 2 de Dockerfile 

Este ejemplo es un poco más complejo que el primero. La finalidad es seguiir mostrando el conjunto de instrucciones que existen para desarrollar un dockerfile. 

A continuación se describe como materializar el ejemplo. 

En línea de comando ejecutar la siguiente intrucción:
```bash
docker build -t examples/example_dockerfile_2 .
```
`-t`es una bandera para el nombre y el punto al final (`.`) indica que el archico dockerfile está en el directorio de trabajo actual. 

Cuando termine la creación de la imagen se puede listarla mediante:
```bash 
docker images
```

Finalmente, para crear un contenedor a partir de la imagen recientemente creada:

```bash
docker run --name example_dockerfile_2 examples/example_dockerfile_2
```

### Otras instrucciones para gestionar la imagen y el contenedor

Para borrar un contenedor hay que realizar dos pasos, primero hay que pararlo y después removerlo: 

```bash 
docker stop example_dockerfile_2 && docker rm example_dockerfile_2
```

Para borrar la imagen se debe ejecutar el siguiente comando:
```bash
docker rmi -f examples/example_dockerfile_2
