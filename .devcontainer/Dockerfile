FROM rust:1.74.1-bookworm

WORKDIR /root

RUN apt-get update && \
  apt-get upgrade -y && \
  rustup component add rustfmt && \
  rustup component add clippy && \
  apt-get install -y zsh && \
  chsh -s /bin/zsh && \
  sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
