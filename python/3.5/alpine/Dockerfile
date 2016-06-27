FROM alpine:3.4

RUN apk add --update python3 wget make && \
    wget --progress=dot:mega --no-check-certificate https://bootstrap.pypa.io/get-pip.py -P /tmp && \
    python3 /tmp/get-pip.py && \
    ln -s /usr/bin/python3 /usr/bin/python && \
    apk del wget && \
    rm -rf /var/cache/apk/* /tmp/* /usr/lib/python*/ensurepip /root/.cache
