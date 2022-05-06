## Airflow local playground

- see https://airflow.apache.org/docs/apache-airflow/stable/start/docker.html



### Instructions

- sed -i "s/AIRFLOW_UID=.*/AIRFLOW_UID=$(id -u)/" .env                # Only relevant for *nix based systems, not Windows
- docker-compose up airflow-init                                      # one-off command, for the first run, not needed afterwards
- docker-compose up -d
- access webserver - http://localhost:8080
- to bring down:
    - docker-compose down
- to bring down and delete postgres volume
    - docker-compose down --volumes
