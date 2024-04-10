# Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Hosting](#hosting locally)
4. [Setup](#setup)

# Introduction

This tutorial will guide you through the steps of setting up a CTFd server. The CTFd code can be found [here](https://github.com/CTFd/CTFd). Online documentation can be found here [here](https://docs.ctfd.io).

If you want to host through CTFd, you can skip to [Hosting Remotely Through CTFd](#hosting-remotely-through-ctfd)

# Installation

The first step is to clone this repository. If you are new to using SSH, you can access [this](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/managing-deploy-keys#set-up-deploy-keys) tutorial for help setting up a key.

Clone this repository with the following command (if you have python 3 and python 2 installed, you might need to use pip3):
```sh
git clone https://github.com/evanmarlo/CTFd-Tutorial.git
```
Change directories into the submodule:
```sh
cd CTFd
```
Clone the CTFd submodule:
```
git submodule init
git submodule update
```
Then install dependencies (might take a minute):
```sh
pip install -r requirements.txt
```

Next, you will need to install Docker [here](https://docs.docker.com/install/).

If your do not already have Docker Compose installed, install it [here](https://docs.docker.com/compose/install/).

# Hosting Locally
Start Docker with the following command:
```
docker run -p 8000:8000 -it ctfd/ctfd
```

While docker is running, open up the following URL in a web browser:
http://localhost:8000/setup

From there you can follow the [Setup](#setup) instructions to setup your CTF. When you are done you can close the container through the terminal by pressing control + c. You can also run and close your container through the docker desktop app. This is how you will save changes to your CTF. See the screenshot below.

![](screenshot1.png)

# Self Hosting

# Hosting Remotely Through CTFd



# Setup