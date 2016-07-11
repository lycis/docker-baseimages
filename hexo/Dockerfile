FROM node:4
MAINTAINER daniel@deder.at

ENV HEXO_PORT=4000

WORKDIR /var/lib/blog/
RUN npm install hexo-cli -g
RUN hexo init
RUN npm install
CMD hexo server -p $HEXO_PORT

EXPOSE 80
HEALTHCHECK --interval=5m --timeout=5s CMD curl -f http://localhost/ || exit 1
