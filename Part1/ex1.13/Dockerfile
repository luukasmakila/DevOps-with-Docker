FROM golang:1.16

WORKDIR /app

COPY ./example-backend .

ENV PORT=8080

ENV REQUEST_ORIGIN=http://localhost:5000

RUN go build

CMD [ "./server" ]