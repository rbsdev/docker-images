FROM python:3.7-alpine3.9

RUN apk add --no-cache tzdata
RUN cp /usr/share/zoneinfo/GMT-0 /etc/localtime
RUN echo "GMT-0" > /etc/timezone
RUN apk del tzdata

RUN apk add --no-cache --virtual .build-deps gcc musl-dev libffi-dev openssl-dev
RUN apk add --no-cache git curl

CMD [ "python", "-dutt", "app.py" ]

WORKDIR /app
