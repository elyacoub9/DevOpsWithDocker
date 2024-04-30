FROM golang:1.16-alpine

WORKDIR /mydir

COPY . .

RUN go build

EXPOSE 8080

CMD [ "./server" ]
      