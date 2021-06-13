## Python Fastapi Template

### Features

* It uses [FastAPI](https://fastapi.tiangolo.com/) framework for API development. FastAPI is a modern, highly performant, web framework for building APIs with Python 3.6+.

* The APIs are served with [Uvicorn](https://www.uvicorn.org/) server. Uvicorn is a lightning-fast "ASGI" server. It runs asynchronous Python web code in a single process.

* [Gunicorn](https://gunicorn.org/) is used here to manage Uvicorn and run multiple of these concurrent processes. That way, you get the best of concurrency and parallelism.

* OAuth2 (with hashed password and Bearer with JWT) based authentication

* [CORS (Cross Origin Resource Sharing)](https://fastapi.tiangolo.com/tutorial/cors/) enabled.

* Flask inspired divisional folder structure better decoupling and encapsulation. This is suitable for small to medium backend development.

* Dockerized using [uvicorn-gunicorn-fastapi-docker](https://github.com/tiangolo/uvicorn-gunicorn-fastapi-docker). This image will set a sensible configuration based on the server it is running on (the amount of CPU cores available) without making sacrifices.

### Run From Commandline
* Go to your project folder and run

    ```bash
    $ export PYTHONPATH="./app"
    $ uvicorn main:app --host 0.0.0.0
    ```


### Run the Containers

* Go to your project folder and run:

    ```bash
    docker-compose up -d
    ```
