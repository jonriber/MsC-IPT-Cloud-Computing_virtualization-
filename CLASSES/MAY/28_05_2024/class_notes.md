# MAY, 28, 2024 - Docker class

## Docker archtecture

client:
    Instaracting with 

    docker build
    docker pull - download images from registry
    docker run - also download and runs imagem from registry
    docker push
    docker login

docker host
    docker daemon
    containers 
    images

registry

    Stores docker images
    docker hub is a public registry open for everyone
    by default, docker checks up for images on `docker hub`
    nginx
    image manager

Docker objects

    Building blocks that are created and used 

Docker Images

    read-only template with instructions for creating a Docker container
    One could create a new image, based on another one (this is pretty common)

    Create a Docker file which defines steps to create and run the image

Docker Container

    A runnable instance of an image

    create, started, stopped, moved, deleted

    connected to networks, attached to starage

    New images can be created from an existing container (current state)

Docker networks

Docker Volumes

    way to persist and share data between containers and host machine

    Allows data to be retainer even if container is deleted

    Why volumes?

    - data persistence
    - data sharing
    - Integrated with host

    Volume types:

    - named volumes
    - bind volumes
    - tpmfs volumes

    Creating a volume

    - docker volume create name_of_volume
    - docker volume ls
    - docker run -d -v my_volume:/data name_of_image
    - docker run -d -v ./host/path:/container/path my_image_name