# Jupyter Notebook Streamlit Python Stack

Available at [Dockerhub](https://hub.docker.com/r/john77eipe/streamlit-notebook)

GitHub Actions in the <https://github.com/jupyter/docker-stacks> project builds and pushes this image to Docker Hub.

Please visit the project documentation site for help to use and contribute to this image and others.

This is built from `jupyter/base-notebook`.

[Jupyter Docker Stacks on ReadTheDocs](https://jupyter-docker-stacks.readthedocs.io/en/latest/index.html)

Usage:

- Running the container

```sh
docker run -it 8501:8501 -v [your local workspace path]:/home/jovyan john77eipe/streamlit-notebook
```

- Use the relate path to the containers work directory in your code

```py
import os 
dir_path = os.path.dirname(os.path.realpath(__file__))
# somewhere in your code
data = pd.read_csv(f"{dir_path}/uber-raw-data-sep14.csv.gz", nrows=100000)
```

The above code snippet is taken from a [streamlit demo](https://github.com/streamlit/demo-uber-nyc-pickups)

- Rebuilding the image (if you need to)

```sh
cd streamlit-notebook
docker build -t john77eipe/streamlit-notebook .
```
