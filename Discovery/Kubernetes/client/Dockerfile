FROM golang:1.12.7-alpine

ENV SOURCES /go/src/github.com/ragagit/Discovery/Kubernetes/
COPY . ${SOURCES}

RUN cd ${SOURCES}client/ && CGO_ENABLED=0 go build

WORKDIR ${SOURCES}client/
CMD ${SOURCES}client/client
