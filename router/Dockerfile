FROM alpine:latest

RUN apk update && apk add fish
RUN ln -s /usr/bin/fish /bin/fish

RUN apk update && apk add bridge-utils

VOLUME [ "/etc" ]

CMD [ "/bin/fish" ]