ARG VARIANT=latest
FROM oven/bun:${VARIANT}

RUN apt-get update \
    && chsh -s $(which bash) bun \
    && apt-get -y install git \
    && apt-get auto-remove -y \
    && apt-get clean -y