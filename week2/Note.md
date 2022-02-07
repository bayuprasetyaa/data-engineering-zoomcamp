# Week 2 - Note
====================================================

### Airflow Setup
- Rename "key.JSON" -> "google_credential.json"
- Make directory for google credential and Move "google_credential.json" to the directory
``` bash
    cd ~ && mkdir -p ~/.google/credentials/
    mv <path/to/your/service-account-authkeys>.json ~/.google/credentials/google_credentials.json
```
- Make dag, los, plugins directory
``` bash
mkdir -p ./dags ./logs ./plugins
echo -e "AIRFLOW_UID=$(id -u)" > .env
```
- Import Airflow 
``` bash
    curl -LfO 'https://airflow.apache.org/docs/apache-airflow/stable/docker-compose.yaml'
```
- Create the requirments.txt
- Build the image
``` bash
    docker-compose build
```
- create "Data_ingestion_gcs" script in "dags"
