FROM openjdk:11-slim

RUN apt-get update \
  && apt-get install -y curl \
  && rm -rf /var/lib/apt/lists/

WORKDIR /app
