# Jupyter Notebook Pyspark Snowpark Python Stack

Available at [Dockerhub](https://hub.docker.com/r/john77eipe/pyspark-snowpark-notebook)

GitHub Actions in the <https://github.com/jupyter/docker-stacks> project builds and pushes this image to Docker Hub.

Please visit the project documentation site for help to use and contribute to this image and others.

This is built from `jupyter/scipy-notebook:python-3.8.8` because snowpark supports only Python 3.8.x.

[Jupyter Docker Stacks on ReadTheDocs](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)

Usage:

- Running the container

```sh
docker run -it -p 8888:8888 -v [your local workspace path]:/home/jovyan/work john77eipe/pyspark-snowpark-notebook
```

- Rebuilding the image (if you need to)

```sh
cd pyspark-snowpark-notebook
docker build -t john77eipe/pyspark-snowpark-notebook .
```