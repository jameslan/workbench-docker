FROM debian:buster

RUN set -ex; \
  apt update; \
  apt remove -y python python-minimal python2 python2.7 python2.7-minimal; \
  update-alternatives --install /usr/bin/python python /usr/bin/python3 1; \
  apt install -y git zsh neovim curl \
    openssh-server \
    default-jdk ocaml-nox opam nodejs npm python3-distutils python3-pip python3-setuptools; \
  rm -rf /var/lib/apt/lists/*; \
  rm -rf /var/cache/apt
