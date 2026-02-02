FROM alpine:latest

RUN apk add --no-cache nginx 

COPY conf/nginx.conf /etc/nginx/nginx.conf
COPY html/index.html /usr/share/nginx/html/index.html

EXPOSE 8080
USER nginx
CMD ["nginx", "-g", "daemon off;"]