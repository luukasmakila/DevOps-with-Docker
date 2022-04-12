#frontend dockerfile
FROM node:16

EXPOSE 5000

COPY ./example-frontend .

RUN npm install

ENV REACT_APP_BACKEND_URL=http://localhost:8080

RUN npm run build

RUN npm install -g serve

CMD [ "serve", "-s", "-l", "5000", "build" ]

#backend dockerfile
FROM golang:1.16

WORKDIR /app

COPY ./example-backend .

ENV PORT=8080

ENV REQUEST_ORIGIN=http://localhost:5000

RUN go build

CMD [ "./server" ]