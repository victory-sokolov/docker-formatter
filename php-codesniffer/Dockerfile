FROM php:8.1-cli-alpine

RUN curl -sSL https://squizlabs.github.io/PHP_CodeSniffer/phpcbf.phar -o phpcbf.phar
RUN chmod a+x phpcbf.phar && mv phpcbf.phar /usr/local/bin/phpcbf

WORKDIR /code

ENTRYPOINT ["phpcbf"]
