FROM alpine:latest
MAINTAINER daniel@deder.at

# install packages
RUN apk add --update ruby

# no rdoc for default
RUN echo gem: --no-document > ~/.gemrc

# install gems
RUN gem install bundler
