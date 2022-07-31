# Use the latest Alpine parent image
FROM alpine
# set th working directory inside the container
WORKDIR /home/Folli
# copy current project directory to workdir
COPY . /home/Folli
# install support packages
RUN apk add make && \
    apk add gcc && \
    apk add libc-dev && \
    make folli  && \
    make test
# run the test script
CMD ["/bin/sh"]

