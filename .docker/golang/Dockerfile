FROM golang:latest as builder
RUN mkdir /app
COPY hello-world.go /app/
WORKDIR /app
RUN go build -o main .


FROM scratch

COPY --from=builder /app /app
CMD ["/app/main"]

