FROM golang:1.18-alpine

RUN mkdir /app

RUN addgroup -S shintagroup
RUN adduser -S -D -h /app shintauser shintagroup
RUN chown -R shintauser:shintagroup /app
USER shintauser

COPY main.go /app

EXPOSE 8080
CMD go run /app/main.go