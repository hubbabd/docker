FROM python:3.6-slim

RUN apt-get update && \
    apt-get install -y \
    curl

RUN curl -L -o /usr/local/bin/param-inject https://github.com/rbi13/aws-param-inject/releases/download/0.0.2/aws-param-inject-linux-amd64 && \
    chmod +x /usr/local/bin/param-inject

ENTRYPOINT ["param-inject"]
CMD ["echo","no command specified"]