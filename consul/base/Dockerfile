#
# Docker base image for consul operations.
#
FROM alpine:latest
MAINTAINER daniel@deder.at

ENV CONSUL_VERSION 0.6.3

RUN apk add --update ca-certificates

RUN wget https://releases.hashicorp.com/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_amd64.zip \
 && unzip consul_${CONSUL_VERSION}_linux_amd64.zip \
 && mv consul /bin/ \
 && rm -rf consul_${CONSUL_VERSION}_linux_amd64.zip

ENTRYPOINT ["/bin/consul"]
