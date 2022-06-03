# Project diagram

## I'll use airflow to control the flow of data
## Install airflow with docker
Download airflow YAML file

```
curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.3.1/docker-compose.yaml'
```
## Create dags, logs and plugins folders

```
mkdir ./dags ./logs ./plugins
```
## Create .env file

```
echo -e "AIRFLOW_UID=$(id -u)\nAIRFLOW_GID=0" > .env
```
## Run docker-compose

```
docker-compose up airflow-init
```
## Run docker-compose up
    
```
docker-compose up
```
## Verify that all is working fine

```
docker ps
```

## 1.A scraper that will extract the data from the [Gwent:The Witcher Card Game](https://www.playgwent.com/).
### The scraper will extract the following information:
* Stats of Victorys, Losses, Draws, Winrate, and the number number of games played by each player per faction. 



















### I'm doing this only for fun. I won't get any profit for this project.