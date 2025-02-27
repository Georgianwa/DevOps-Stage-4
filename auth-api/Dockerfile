FROM golang:1.19 as builder

WORKDIR /app
COPY . .
RUN go build -o auth-api

FROM alpine:latest
WORKDIR /root/
COPY --from=builder /app/auth-api .
CMD ["./auth-api"]