FROM alpine:latest

RUN apk update && apk add fish
RUN ln -s /usr/bin/fish /bin/fish

RUN apk update && apk add bridge-utils net-tools

RUN apk update && apk add openrc
RUN apk update && apk add dhcp
RUN cp /etc/dhcp/dhcpd.conf.example /etc/dhcp/dhcpd.conf
RUN rc-update add dhcpd

RUN apk add neovim

VOLUME [ "/etc" ]

CMD [ "init" ]