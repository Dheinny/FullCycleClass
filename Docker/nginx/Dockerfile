FROM nginx:latest

COPY html /usr/share/ngnix/html

ENTRYPOINT [ "docker-entrypoint.sh" ]
CMD [ "nginx", "-g", "daemon off;" ]