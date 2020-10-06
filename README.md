# Flask + SQL + Grafana Docker application
<img src="https://img.shields.io/badge/docker%20-%230db7ed.svg?&style=for-the-badge&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/python%20-%2314354C.svg?&style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/flask%20-%23000.svg?&style=for-the-badge&logo=flask&logoColor=white"/>
<img src="https://img.shields.io/badge/mysql-%230175C2.svg?&style=for-the-badge&logo=mysql&logoColor=white"/>
<img src="https://img.shields.io/badge/grafana%20-%23F37626.svg?&style=for-the-badge&logo=grafana&logoColor=white"/>


This repo consists of a Flask APP, a SQL database and a Grafana Dashboard.

### Flask

Go into the [flaskApp directory](./flaskApp), and type the following command to build the image:
```
docker build -t flask_docker .
```
Then the next one to run a container with it:
```
docker run -d -p 4200:80 --name=flask_container -v $PWD:/app  flask_docker
```
The application will be avaliable in http://localhost:4200

To stop and start again just type:

```
docker stop flask_container
docker start flask_container
```
