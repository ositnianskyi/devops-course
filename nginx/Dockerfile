FROM alpine

RUN apk update && apk add nginx

COPY default.conf /etc/nginx/http.d/default.conf
COPY index.html /usr/share/nginx/html/index.html

EXPOSE 80

STOPSIGNAL SIGQUIT

CMD ["nginx", "-g", "daemon off;"]