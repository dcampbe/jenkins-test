FROM alpine:latest
RUN apk add --update bash curl perl sed && rm -rf /var/cache/apk/*
COPY run_tests.sh /
COPY wait-for-it.sh /
CMD ["bash", "run_tests.sh"]
