FROM ubuntu:20.04

RUN apt-get update ; apt-get install -qq -y curl

COPY script.txt .

RUN chmod +x script.txt

ENTRYPOINT ["./script.txt"]

CMD ["param1"]