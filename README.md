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
