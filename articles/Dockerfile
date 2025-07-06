FROM httpd
LABEL maintainer="ektech"
USER root
RUN apt -y update 
WORKDIR /usr/local/apache2/htdocs/

RUN rm -rf *
COPY .  /usr/local/apache2/htdocs/

ENTRYPOINT ["httpd-foreground"]
EXPOSE 80
