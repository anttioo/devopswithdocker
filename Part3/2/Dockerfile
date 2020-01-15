FROM python:3.5-alpine

RUN apk add --no-cache gcc make ffmpeg libxml2-dev libxslt-dev musl-dev py-lxml py-setuptools \
    && pip3 install --user --upgrade yle-dl
WORKDIR /app
ENTRYPOINT ["/root/.local/bin/yle-dl"]