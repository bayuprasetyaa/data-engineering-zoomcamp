# Problems
## Some problems that my be found
===
### 1. Resolving invalid docker-compose.yaml error during using Airflow with Docker
``` bash
docker-compose up airflow-init
ERROR: The Compose file './docker-compose.yaml' is invalid because:
Unsupported config option for services.airflow-cli: 'profiles'
Invalid top-level property "x-airflow-common". Valid top-level sections for this Compose file are: version, services, networks, volumes, and extensions starting with "x-".
``` 
**Solution** : Need to upgrade 'docker-compose' version

### 2. 
"Unable to write file '/home/bayu/DataTalks/week2/airflow/dags/data_ingestion_gcs_dags.py' (NoPermissions (FileSystemError): Error: EACCES: permission denied, open '/home/bayu/DataTalks/week2/airflow/dags/data_ingestion_gcs_dags.py')"
**Solution** : Give permission rwx(read, write, excute) for other user 