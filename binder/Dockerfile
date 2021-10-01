#
#  This Dockerfile creates a docker image from the base image jupyter/minimal-notebook (https://hub.docker.com/r/jupyter/minimal-notebook)
#
ARG almond_version=0.10.9
ARG scala_kernel_version=2.12.12
FROM almondsh/almond:$almond_version-scala-$scala_kernel_version
USER jovyan
RUN /bin/bash -c "pip install Jupyterlab --upgrade"
RUN /bin/bash -c "jupyter labextension install jupyterlab-plotly"
