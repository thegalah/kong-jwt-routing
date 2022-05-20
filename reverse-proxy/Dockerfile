FROM nginx:1.15.0-alpine
RUN apk update && apk add openssl
COPY nginx.conf /etc/nginx/nginx.conf
COPY site.conf /etc/nginx/site.conf
