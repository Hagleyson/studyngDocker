FROM nginx:latest

WORKDIR /app

RUN apt-get update && \ 
    apt-get install nano -y

COPY html /usr/share/nginx/html

ENTRYPOINT [ "/docker-entrypoint.sh" ]
CMD [ "nginx","-g","daemon off;" ]