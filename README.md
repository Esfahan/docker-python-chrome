## docker-python-chrome
Python with headless chrome on CentOS7(Docker)

- chromedriver_linux64 2.43
- google-chrome-stable 70.0.3538.77
- Python 3.7.1

## DockerHub
- https://hub.docker.com/r/esfahan/python-chrome

## docker build

```
$ sudo docker build -t python-chrome:latest ./
```

## docker run

```
$ sudo docker run --name python-chrome-container \
                  -v $(pwd)/code:/code \
                  -itd python-chrome:latest /bin/bash
```

## Usage

```
$ sudo docker exec -it python-chrome-container /bin/bash -c 'python /code/main.py'
Google
```
