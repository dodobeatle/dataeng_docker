## Para ejecutar
```bash
# Crear directorio para configuraciones
mkdir -p nginx/conf.d ssl

# Copiar los archivos de configuración
# Colocar nginx.conf en el directorio actual

# Iniciar los servicios
docker-compose up -d
```

## Acceso a los servicios:
* Zabbix: http://localhost/zabbix
Usuario: Admin
Contraseña: zabbix
* Portainer: 
    * http://localhost/portainer
    * Crear credenciales en el primer inicio
* CheckMK: 
    * http://localhost/checkmk
    * Usuario: cmkadmin
    * Contraseña: cmk123

## Notas importantes:
1. Ajusta las contraseñas antes de implementar en producción
2. Considera agregar SSL para producción
3. Ajusta las zonas horarias según tu ubicación
4. Los volúmenes persistirán los datos
5. Asegúrate de tener suficientes recursos en tu máquina

## Para gestionar:

```bash
# Ver logs
docker-compose logs -f [servicio]

# Reiniciar un servicio
docker-compose restart [servicio]

# Detener todo
docker-compose down

# Detener y eliminar volúmenes
docker-compose down -v
```




