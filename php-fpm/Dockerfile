FROM gcr.io/stacksmith-images/ubuntu:14.04-r8
MAINTAINER Bitnami <containers@bitnami.com>

ENV BITNAMI_IMAGE_VERSION=7.0.6-r1 \
    BITNAMI_APP_NAME=php-fpm \
    BITNAMI_APP_USER=daemon

RUN bitnami-pkg unpack php-7.0.6-0 --checksum 8ca32e21642fbe2fd23cdf7459d6cb4b65bb1b89b0e230333c8da553135d79a6
RUN mkdir -p /bitnami && ln -sf /bitnami/php /bitnami/php-fpm
ENV PATH=/opt/bitnami/php/sbin:/opt/bitnami/php/bin:/opt/bitnami/common/bin:$PATH

VOLUME ["/bitnami/$BITNAMI_APP_NAME"]

WORKDIR /var/www/abenyu

EXPOSE 9000
