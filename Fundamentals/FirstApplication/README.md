# First Application

Building first application is divided into 2 parts:
- Ops Section
- Dev Section

## Description
In the Ops section i; downloaded a Docker image, launched a
container from it, logged into the container, executed a command inside of it, and
then stopped and deleted the container.
In the Dev section, i containerized a simple application by pulling some source
code from GitHub and building it into an image using instructions in a Dockerfile.
i then ran the containerized app (psweb).

## Commands

```sh
git clone git@github.com:nigelpoulton/psweb.git
cd psweb
docker image build -t test:latest .
docker container run -d --name web1 --publish 8080:8080 test:latest
```
Open a web browser and navigate to the localhost:8080. You will see the web page.

