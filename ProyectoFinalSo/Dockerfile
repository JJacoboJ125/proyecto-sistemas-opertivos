# Usar una imagen base de Ubuntu
FROM ubuntu:20.04

ENV DEBIAN_FRONTEND=noninteractive

# Instalar las dependencias necesarias
RUN apt-get update && apt-get install -y \
    build-essential \
    gcc \
    python3 \
    python3-pip \
    curl \
    vim \
    nano \
    x11-apps \
    xfce4 \
    xfce4-terminal \
    bc \
    && rm -rf /var/lib/apt/lists/*

RUN apt-get update && apt-get install -y curl


RUN apt-get update && apt-get install -y gnome-weather


RUN apt-get update && apt-get install -y gnome-calculator


RUN echo '#!/bin/bash\ncurl wttr.in' > /usr/local/bin/weather && chmod +x /usr/local/bin/weather


RUN echo '#include <stdio.h>\nint main() { printf("Hola, Mundo!\\n"); return 0; }' > /root/hola_mundo.c


RUN echo 'print("Hola desde Python!")' > /root/hola_mundo.py


WORKDIR /root


CMD ["/bin/bash"]
