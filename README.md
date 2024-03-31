# CTFd-Tutorial

This tutorial will guide you through the steps of setting up a CTFd server.

The CTFd code can be found [here](https://github.com/CTFd/CTFd). Online documentation can be found here [here](https://docs.ctfd.io). Clone this repository with the following command:
```sh
git clone https://github.com/CTFd/CTFd.git
```
Then install dependencies:
```sh
pip install -r requirements.txt
```
If you have python 3 and python 2 install, use python3 (pip3):
```sh
pip3 install -r requirements.txt
```

Next, you will need to install Docker [here](https://docs.docker.com/install/).

If your do not already have Docker Compose install, install it [here](https://docs.docker.com/compose/install/).

Start Docker with the following command:
```
docker run -p 8000:8000 -it ctfd/ctfd
```

While docker is running, open up the following URL in a web browser:
http://localhost:8000/setup



git submodule init
git submodule update