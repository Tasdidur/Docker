FROM golang:latest AS primary

WORKDIR /app

COPY go.mod go.sum ./

COPY . .

RUN CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o main .

FROM alpine:latest 

WORKDIR /root/

COPY --from=primary /app/main .

CMD ["./main"]