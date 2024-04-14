FROM ghcr.io/lazka/msys2-docker-experimental

RUN apt update \
    && apt install -y git \
    && rm -rf /var/lib/apt/lists/*

RUN msys2 -c "pacman -S --noconfirm --needed git"

# Link in the injected git config, to make git work in MSYS2 too
RUN ln -s /etc/gitconfig ~/.wine/drive_c/msys64/etc/gitconfig
RUN ln -s /.codespaces ~/.wine/drive_c/msys64/.codespaces
