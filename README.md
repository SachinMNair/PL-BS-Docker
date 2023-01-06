# PL-BS-Docker
This repository allows you to build a PlayWright Docker image and run it from Docker on BrowserStack

## Setup

- Download and install Docker Desktop from https://docs.docker.com/get-docker/ and open the application to start the Docker

- Clone the repo <br>
`git clone https://github.com/SachinMNair/PL-BS-Docker.git`

- Build Docker image <br>
`docker build -t <docker_image_name> .`

- Check if the image is created <br>
`docker image ls`

- Run the docker image that will run PlayWright test on BrowserStack<br>
`docker run --env BROWSERSTACK_USERNAME=<BrowserStack_username> --env BROWSERSTACK_ACCESS_KEY=<BrowserStack_access_key> -it <docker_image_name>:latest npm run test`

## Check your results

- Go to the Automate Dashboard to check the Automation test/build <br>
`http://automate.browserstack.com/`