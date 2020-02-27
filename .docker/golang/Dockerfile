FROM golang:latest
RUN mkdir /app
ADD hello-world.go /app/
WORKDIR /app
RUN go build -o main .
CMD ["/app/main"]
