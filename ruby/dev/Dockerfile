#
# Ruby baseimage with developer tools installed
# base for all other ruby images
#
FROM alpine:latest
MAINTAINER daniel@deder.at

# add default available scripts
ADD ./scripts/ /opt/scripts/

# install packages
RUN apk add --update ruby

# no rdoc for default
RUN echo gem: --no-document > ~/.gemrc
RUN sh /opt/scripts/add_dev.sh

# install gems
RUN gem install bundler
RUN gem install io-console
