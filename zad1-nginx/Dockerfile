FROM nginx:alpine

RUN apk update && \
    apk add --no-cache curl && \
    rm -rf /var/cache/apk/*

COPY index.html /usr/share/nginx/html/index.html

ENTRYPOINT ["nginx"]
CMD ["-g", "daemon off;"]