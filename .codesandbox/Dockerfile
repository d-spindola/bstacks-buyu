FROM ubuntu

WORKDIR /bin

RUN apt update -y && apt install -y unzip curl

ARG BUN_VERSION="bun-v0.7.3"

RUN curl -L -o bun-linux-x64.zip "https://github.com/oven-sh/bun/releases/download/$BUN_VERSION/bun-linux-x64.zip"
RUN unzip -j bun-linux-x64.zip && rm bun-linux-x64.zip

WORKDIR /workspace
