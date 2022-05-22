FROM kong:2.8.1-alpine
USER root

RUN luarocks install kong-jwt2header
USER kong

COPY kong.yml /etc/kong/kong.yml
