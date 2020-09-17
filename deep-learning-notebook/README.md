# Deep Learning Notebook

## Additional Packages Included

1. plotly - for making beautiful visualizations
2. streamlit - for making beautiful, ML based web apps easily
3. pytorch - another deep learning library for python, apart from tensorflow
3. The Jupyter Lab extension for plotly graphs to render properly in Jupyter Lab

## Build instructions

Run the following command in the terminal to build the image

```
docker build -t <any name you want> . # Do not forget the '.' at the end
```

Skip this step if you have already pulled the image from the Docker Hub repository

## Run instructions

Run the following command to fire up the docker container for the first time

```
docker run -it -v "$PWD":/home/jovyan/work --name <any name you want> -p 8888:8888 <the tag name you gave while building the image> bash
```

You can now launch Jupyter Notebook, by just typing in the command `jupyter notebook` in the shell. If you want to exit the Jupyter Notebook server, Ctrl+C, does that for you, and if you want to exit the shell of the container, just type the command `exit` and you should see your prompt string change back to its original value.

To run the container again, use the following commands

```
docker start <the name you gave to the --name flag while running the container in the previous step>
docker exec -it <name you provided to the --name flag in the previous command> bash
```

Or you can also run the start.sh script (you can change the name of your container in the .sh file) with the following commands

```
chmod +x start.sh # This is to allow the start.sh file to be executed
./start.sh
```

As usual, you can type `jupyter notebook` here and a Jupyter Notebook server fires up.
