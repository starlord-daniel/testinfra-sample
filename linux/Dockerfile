FROM python:3.8.6-alpine

COPY . linux/.

WORKDIR /linux

# install make
RUN apk update && apk add make

# run the init, lint and tests with make
RUN make test

CMD ["make", "run"]