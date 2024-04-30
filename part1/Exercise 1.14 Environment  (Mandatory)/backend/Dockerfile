FROM golang:1.16-alpine

WORKDIR /mydir

COPY . .

RUN go build

EXPOSE 8080

ENV REQUEST_ORIGIN=http://10.10.10.100:5000

CMD [ "./server" ]
      