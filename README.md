# Dockerfiles

- This repository contains all my Dockerfiles, that I use regularly.
- These Dockerfiles are just slight modifications of the Dockerfiles provided by Jupyter, so as to include some extra packages that I like.

You can use these Dockerfiles to create your own image, or you can just pull the images from Docker Hub [here](https://hub.docker.com/repository/docker/anandrajaram21/jupyter-environments)

## How to use the images from Docker Hub

You can pull the image of your choice from Docker Hub with the following command

```
docker pull <image tag>
```

After pulling the image, read the README.md file in the corresponding folder (with the same name as that of the image that you pulled, for example, navigate to deep-learning-notebook if you pulled the image with the tag anandrajaram21/jupyter-environments:deep-learning)

## All the Dockerfiles here are based on the images provided by the Jupyter Team on Docker over [here](https://jupyter-docker-stacks.readthedocs.io/en/latest/#). So huge thanks to them for providing us with such brilliant Docker images to build upon.
