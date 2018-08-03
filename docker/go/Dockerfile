FROM golang:latest

RUN apt-get update -qq && apt-get install vim -y

WORKDIR /go
ADD . /go

RUN go get -u github.com/oxequa/realize

EXPOSE 8080

CMD ["go", "run", "main.go"]
