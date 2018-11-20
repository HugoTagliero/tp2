# Answers

Nom: Tagliero
Prénom: Hugo
NB: 4

## 1.3
command: docker build -t monscript .

## 1.4
answer: les ports sont fermés
command: docker run -p 8080:8080 monscript

## 1.5
command: docker run -p 8080:8080 -e ENVIRONMENT=python:3-alpine monscript

## 1.6
answer: Parce qu'elle n'a pas le bon nom.
command: docker tag monscript htagliero/tp2-docker:0.1 
puis: docker push htagliero/tp2-docker:0.1

## 1.7
answer: Docker ne trouve pas l'image locale donc il la télécharge.
command: sudo docker rmi -f $(docker images -q)
command: docker run -p 8080:8080 -e ENVIRONMENT=python:3-alpine htagliero/tp2-docker
command: docker run -p 8080:8080 -e ENVIRONMENT=python:3-alpine -d htagliero/tp2-docker

## 1.8
answer: nom du container : hopeful_proskuriakova, id : 1702ff909853
command: docker ps
command: docker rename 1702ff909853 containertp2

## 1.9
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=16.04
DISTRIB_CODENAME=xenial
DISTRIB_DESCRIPTION="Ubuntu 16.04.5 LTS"
NAME="Ubuntu"
VERSION="16.04.5 LTS (Xenial Xerus)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 16.04.5 LTS"
VERSION_ID="16.04"
HOME_URL="http://www.ubuntu.com/"
SUPPORT_URL="http://help.ubuntu.com/"
BUG_REPORT_URL="http://bugs.launchpad.net/ubuntu/"
VERSION_CODENAME=xenial
UBUNTU_CODENAME=xenial


## 1.11
command: sudo docker run -d -p 1010:1010 -e APP_PORT=1010 -e WS_BACK_URL=172.17.0.1 htagliero/tp2-docker


## 2.1
command: command: docker-compose up


## 2.6
command: 
command:

