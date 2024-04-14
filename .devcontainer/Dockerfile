FROM ghcr.io/lazka/msys2-docker-experimental

RUN apt update \
    && apt install -y git \
    && rm -rf /var/lib/apt/lists/*

RUN msys2 -c "pacman -S --noconfirm --needed git"
