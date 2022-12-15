FROM postgres:11.18-bullseye

# Install the plpython extension based on the PG_MAJOR version defined in the parent image
RUN apt-get update -q
RUN apt-get upgrade
RUN apt-get update \
 && apt-get install -y postgresql-contrib postgresql-plpython3-11 \
 && rm -rf /var/lib/apt/lists/*
 