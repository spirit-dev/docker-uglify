ARG alpine_version

FROM gitlab-registry-internal.spirit-dev.net/infrastructure/docker/alpine:${alpine_version}

ARG alpine_version

LABEL alpine_version="${alpine_version}" \
    spiritdev_official="yes" \
    layer="1" \
    from="gitlab-registry-internal.spirit-dev.net/infrastructure/docker/alpine" \
    maintainer="bordat.jean@gmail.com"

RUN apk add --no-cache npm=9.6.6-r0 wget=1.21.4-r0 && \
    npm install uglify-js uglifycss -g
