# syntax=docker/dockerfile:1

FROM --platform=$TARGETPLATFORM alpine:3.18

WORKDIR /app

RUN echo "#!/usr/bin/env sh" >> ./entrypoint.sh
RUN echo "echo 'RELEASE directory'" >> ./entrypoint.sh
RUN chmod +x ./entrypoint.sh

ENTRYPOINT ["./entrypoint.sh"]
