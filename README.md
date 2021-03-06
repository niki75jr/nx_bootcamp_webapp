
## Homework #2:  🐳🌐  Docker-Nginx Site

<p align="center">Simple static site ("<a href="https://www.docker.com/" target="_blank">docker</a>" + "<a href="https://nginx.org/en/" target="_blank">nginx</a>" + "<a href="https://www.mkdocs.org/" target="_blank">mkdocs</a>")</p>

##  Getting Started

**[Jenkins-version](https://github.com/niki75jr/nx_bootcamp_webapp/tree/jenkins)**

### Requirements (for Ubuntu)

##### Docker
   
    sudo apt update
    sudo apt install docker.io

##### Docker-compose
   
    sudo apt update
    sudo apt install docker-compose
    
### Installation

    curl -L https://github.com/niki75jr/nx_bootcamp_webapp/archive/refs/tags/v0.1.1.tar.gz | tar xz
    cd nx_bootcamp_webapp-0.1.1
    docker-compose build

### Launch

    docker-compose up -d
    
### Usage

To start the site, run the command `docker-compose up -d`, the application will start in detached mode. 
To change the site content, go to the site management image `docker exec -it managesite bash` and change the content following the <a href="https://www.mkdocs.org/" target="_blank">instructions</a>, or change the contents of the "**data**" directory.

Open the page in the browser at the address `localhost` or the ip address of your host machine.

### Commands

`docker-compose up -d`  - launch the site in an detached mode

### Images

 1. **managesite** (size: **201 MB**)
 2. **nginx:1.19.10-alpine** (size: **22.6 MB**)
