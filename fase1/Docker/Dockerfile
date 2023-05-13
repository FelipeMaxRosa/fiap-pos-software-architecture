FROM ubuntu:latest

RUN apt-get update
RUN apt-get install nginx -y

VOLUME [ "/var/www/html" ]
WORKDIR "/var/www/html"

# ADD index.html index.html
COPY index.html index.html

ENTRYPOINT [ "/usr/sbin/nginx", "-g", "daemon off;" ]

EXPOSE 80

# ADD "https://images.pexels.com/photos/1521304/pexels-photo-1521304.jpeg" "foto.jpeg"

# # Como baixamos o arquivo precisamos alterar a # permissão para que seja possível acessá-lo
# RUN chmod644 foto.jpeg
# ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]