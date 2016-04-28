##### how to use:
# docker build -t infrared/f23 f23
# docker run -it --rm infrared/f23 /bin/bash -c 'cd /infrared; ir-provisioner --help'
# ... or cut after /bin/bash and do it interactively

FROM fedora
MAINTAINER psedlak

RUN dnf install -y python-pip git python-devel gcc redhat-rpm-config
RUN git clone https://github.com/rhosqeauto/InfraRed.git /infrared

RUN cd /infrared; pip install -e .

