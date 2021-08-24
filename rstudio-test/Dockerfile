FROM rocker/rstudio:latest

# install stuff

USER root

WORKDIR /data

#RUN echo "rsession-which-r=/data/conda/bin/R" > /etc/rstudio/rserver.conf

COPY .rs-setup .

RUN bash .rs-setup
