FROM nginx:latest

RUN apt-get update && \ 
    apt-get install libzip-dev -y && \
    apt-get install vim

COPY html /usr/share/nginx/html

CMD ["nginx", "-g", "daemon off;"]

ENTRYPOINT [ "server" ]
CMD [ "--host=0.0.0.0" ]
