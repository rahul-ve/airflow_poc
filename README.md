## Airflow local playground

- see https://airflow.apache.org/docs/apache-airflow/stable/start/docker.html



### Instructions

- sed -i "s/AIRFLOW_UID=.*/AIRFLOW_UID=$(id -u)/" .env
- docker-compose up airflow-init
- docker-compose up -d
- access webserver - http://localhost:8080
