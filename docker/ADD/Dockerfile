FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/jitheshl/terraform-expense-dev-infra/refs/heads/main/00-vpc/vpc.tf /usr/share/nginx/html/index.html
RUN chmod +r /usr/share/nginx/html/index.html
CMD ["nginx","-g","daemon off;"]