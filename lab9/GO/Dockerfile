FROM golang:1.21-alpine
WORKDIR /GO
COPY go.mod .
RUN go mod download
COPY main.go .
RUN go build -o app .
EXPOSE 8080
CMD ["./app"]

