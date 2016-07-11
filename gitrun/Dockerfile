FROM debian:stable
MAINTAINER daniel@deder.at

RUN apt-get update && apt-get install -y git
CMD git clone $GIT_RUN_REPO target && cd target && ./target/run.sh
