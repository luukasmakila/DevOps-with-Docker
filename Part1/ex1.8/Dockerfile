FROM ubuntu:20.04

RUN apt-get update ; apt-get install -qq -y curl

COPY prevScript.sh .

RUN chmod +x prevScript.sh

CMD ./prevScript.sh