FROM golang:1.24.0

LABEL description="Golang - HTMX"

WORKDIR /app

COPY . .

RUN go mod download

RUN CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -o ./main

ENTRYPOINT ["./main"]
