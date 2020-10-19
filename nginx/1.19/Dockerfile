FROM nginx:1.19-alpine

RUN apk add --no-cache curl # add curl to use healthcheck
COPY config.conf /etc/nginx/conf.d/default.conf.tmpl
COPY run.sh /usr/local/bin/

EXPOSE 8080

CMD run.sh