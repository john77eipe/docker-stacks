# Jupyter Notebook Snowpark Python Stack

Available at [Dockerhub](https://hub.docker.com/r/john77eipe/snowpark-notebook)

GitHub Actions in the <https://github.com/jupyter/docker-stacks> project builds and pushes this image to Docker Hub.

Please visit the project documentation site for help to use and contribute to this image and others.

- [Jupyter Docker Stacks on ReadTheDocs](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)
- [Selecting an Image :: Core Stacks :: jupyter/snowpark-notebook](https://jupyter-docker-stacks.readthedocs.io/en/latest/using/selecting.html#jupyter-snowpark-notebook)

This is built from `scipy-notebook:python-3.8.8` since snowpark support only Python 3.8.

Usage:

- Running the container

```sh
docker run -it -p 8888:8888 -v [your local workspace path]:/home/jovyan/work  john77eipe/snowpark-notebook
```

- Rebuilding the image (if you need to)

```sh
cd snowpark-notebook
docker build -t john77eipe/snowpark-notebook .
```
