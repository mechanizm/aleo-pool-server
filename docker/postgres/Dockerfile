FROM postgres:15

# Install the plpython extension based on the PG_MAJOR version defined in the parent image
RUN apt-get update -q
RUN apt-get upgrade
RUN \
# add multicorn/SqlAlchemyFdw foreign table extension and plpython3 with some libraries:
    apt-get -y install python3 && \
    PYTHON=/usr/bin/python3 && \
    apt-get -y install python3-dev python3-pip postgresql-plpython3-15
