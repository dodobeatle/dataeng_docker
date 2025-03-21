# 🚀 ¿Cómo ejecutarlo?
Finalizado la configuración del YAML. Abra un terminal en el mismo directorio y ejecute:

```bash
docker-compose up -d
```

Los servicios que se ejecutarán y de los cuales se puede acceder:

* PostgreSQL → localhost:5432
* MinIO → localhost:9001 (Web UI) / localhost:9000 (S3 API)
* Kafka → localhost:9092
* Airflow → http://localhost:8080
* Spark Master → http://localhost:8081
* Metabase → http://localhost:3000
* Jupyter → http://localhost:8888