FROM armv7:armhf-ubuntu
LABEL maintainer "sorlinV<valentin.sorlin@hotmail.com>"

LABEL caddy_version="0.0.1" architecture="arm"

RUN apk add --no-cache git build-base

# install caddyplug
RUN go get -v github.com/abiosoft/caddyplug/caddyplug \
 && mv /go/bin/caddyplug /usr/bin/caddyplug \
 && /usr/bin/caddyplug list

# install caddy using caddyplug
RUN /usr/bin/caddyplug install-caddy

EXPOSE 80 443 2015
VOLUME .caddy
WORKDIR /srv

COPY Caddyfile /etc/Caddyfile
COPY /home/isidoris-simplon/rendu /srv

ENTRYPOINT ["/usr/bin/caddy"]
CMD ["--conf", "/etc/Caddyfile", "--log", "stdout"]