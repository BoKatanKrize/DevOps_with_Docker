FROM golang:1.16

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

RUN go build
RUN go test ./...

ENTRYPOINT ["./server"]
CMD PORT REQUEST_ORIGIN

# Build container : docker build . -t example-backend
# Run container : docker run -p 8080:8080 example-backend
