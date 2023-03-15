# ProjetCloudComputing

### Cloning this repository

To run this code, you first need to clone it.
Make sur that you have Git install or you have Linux (or at least a Linux VM). Then run the following command :
`git clone <https://github.com/alily23/ProjetCloudComputing.git`>

### Adding some images

This code use additionnal images. Which are mongo and node:16-alpine. So, in order to be sure that this project run, you need to make sure that you have the images with the correct version.
To install them, simply run theses commands : `docker build mongo:latest` and `docker build node:16-alpine`

### Building the docker compose project

You just need now to create the docker images of our projects with the docker-compose.yml file. For this, we simply need to run it. So in the directory of the project, use the commande : `docker-compose build`

### Run the project

Now that the images are all build, you simply have to run the project. For that, you need to write the following commande in the project directory.
`docker-compose up -d`. Then you just have to open [http://localhost:8080](http://localhost:8080/) to use the project.
