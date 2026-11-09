FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD view-source:https://docs.docker.com/engine/install/rhel/ /usr/share/nginx/html/index.html
CMD ["nginx","-g","daemon off;"]