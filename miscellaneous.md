## Docker

Detailed Referance: [Docker](https://www.freecodecamp.org/news/a-beginners-guide-to-docker-how-to-create-your-first-docker-application-cc03de9b639f/?fbclid=IwAR1cLV81eDZqT9o7sqqnuwfPuVvU7Qocy5j6L2_gpRpOaSS7hW7DEgauIGg)

**Q: What can I do with Docker?**

- quickly deploy and scale applications into any environment
- create independent and isolated environments to launch and deploy its applications.
- These environments are then called containers.

**Q: What is a Docker Image?**

- a read-only template that defines your container.
- definitions for any libraries and dependancies the code needs.
- A Docker container is an instantiated (running) Docker image.

**Q: What is the difference between Docker and a virtual machine?**

- Docker is an operating system (or runtime) for containers.
- Unlike Docker, a virtual machine will include a complete operating system. It will work independently and act like a computer.
- Docker will only share the resources of the host machine in order to run its environments.

When Docker file is available, image to contain the application needs to be created.

> ` $ sudo docker build -t lentra/fe-apps -f ./docker/Dockerfile .`


Once the image is created, your code is ready to be launched.

> `$ sudo docker run --network=host lentra/fe-apps`

## Verdaccio

Publish npm package locally.
Use the same to install it in the other projects.

## Linux Terminal commands

ctrl +  u
	+ a
	+ e

touch
open
rm remove
pwd print working directory

## Host Element

Most of the time, the render() function describes the children elements that are about to be rendered, but it can also be used to render attributes of the host element itself.

The Host functional component can be used at the root of the render function to set attributes and event listeners to the host element itself.

## Promise

Object to which callback funcitons can be attatched to.
.then()
- if resolved
.catch()
- if error
.finally()
- when any of the above operations are done
