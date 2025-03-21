# Ejemplo Simple 1 
Este ejemplo es el más sencillo para crear una imagen a partir de una archivo dockerfile. Laintención del mismo es mostrar la estructura básica del dockerfile.

A continuación se describe como materializar el ejemplo. 

En línea de comando ejecutar la siguiente intrucción:
```bash
docker build -t examples/example_simple_1 .
```

Cuando termine la creación de la imagen se puede listarla mediante:
```bash 
docker images
```

Finalmente, para crear un contenedor a partir de la imagen recientemente creada:

```bash
docker run --name ejemplo_1 examples/example_simple_1
```

### Otras instrucciones para gestionar la imagen y el contenedor

Para borrar un contenedor hay que realizar dos pasos, primero hay que pararlo y después removerlo: 

```bash 
docker stop ejemplo_1 && docker rm ejemplo_1
```

Para borrar la imagen se debe ejecutar el siguiente comando:
```bash
docker rmi -f examples/example_simple_1
```