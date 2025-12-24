FROM python:3.15.0a2-trixie

# Install dependencies
ARG DEPS_DIR=/dependencies
COPY ./$DEPS_DIR /mnt/$DEPS_DIR
RUN pip install --no-cache-dir -r /mnt/$DEPS_DIR/pip.txt

COPY ./src /app/
WORKDIR /app

ENTRYPOINT [ "/bin/bash" ]