FROM golang:1.10.2-alpine
LABEL maintainer="will835559313@163.com"
COPY . /app
WORKDIR /app
RUN apk update && apk add git \
    && go get github.com/gin-gonic/gin \
    && go build \
    && rm -rf /go
EXPOSE 80
CMD ["./app"]