# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.ARG BASE_CONTAINER=jupyter/scipy-notebook
FROM $BASE_CONTAINER

LABEL maintainer="Jupyter Project <jupyter@googlegroups.com>"

# Install Tensorflow
RUN pip install --quiet --no-cache-dir \
    'tensorflow==2.2.0' && \
    fix-permissions "${CONDA_DIR}" && \
    fix-permissions "/home/${NB_USER}"

RUN pip install --quiet --no-cache-dir torch torchvision

RUN pip install --quiet --no-cache-dir plotly

RUN pip install --quiet --no-cache-dir streamlit

RUN pip install --quiet --no-cache-dir keras-tuner
 
RUN jupyter labextension install jupyterlab-plotly@4.10.0

RUN pip install --quiet --no-cache-dir statsmodels==0.12.0
