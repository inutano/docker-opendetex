FROM ubuntu:18.04
ENV OPENDETEX_VERSION=2.8.1
RUN apt update -y && apt install -y make gcc flex wget
RUN wget https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/opendetex/opendetex-${OPENDETEX_VERSION}.tar.bz2 && \
    tar xjvf opendetex-${OPENDETEX_VERSION}.tar.bz2 && \
    cd opendetex && \
    make && make install
CMD ["detex"]

