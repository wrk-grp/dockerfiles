FROM --platform=linux/amd64 bitnami/minideb:latest AS builder

# install_packages vs apt install is a minideb specific way to optimize
# the layer growth when installing packages.
RUN install_packages neovim

WORKDIR /app
COPY . .

CMD [ "nvim", "." ]

