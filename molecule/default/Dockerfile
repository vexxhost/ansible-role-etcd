FROM docker.io/ubuntu:focal

RUN \
  apt-get update && \
  apt-get install -y \
    ca-certificates \
    iproute2 \
    python3 \
    python3-cryptography

ADD https://raw.githubusercontent.com/gdraheim/docker-systemctl-replacement/master/files/docker/systemctl3.py /usr/bin/systemctl
RUN chmod +x /usr/bin/systemctl
CMD ["/usr/bin/systemctl", "--init"]
