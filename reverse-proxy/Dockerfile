FROM nginx:1.21.6-alpine
RUN apk update && apk add openssl
COPY nginx.conf /etc/nginx/nginx.conf
COPY site.conf /etc/nginx/site.conf
RUN openssl req -new -newkey rsa:2048 -days 3650 -nodes -x509 -subj "/C=AU/ST=NSW/L=Sydney/O=GoCoderone/CN=app.gocoderone.dev" -keyout /etc/nginx/server.key -out /etc/nginx/server.crt
