FROM --platform=windows/amd64 python:3.10-rc

COPY . windows/.

WORKDIR /windows

# run the init, lint and tests with make
RUN make test

CMD ["make", "run"]