FROM httpd:2.4

COPY ./public-html/ /usr/local/apache2/htdocs/

EXPOSE 80

RUN mkdir /etc/apache2

RUN mkdir /usr/sbin/apache2ctl

RUN chmod 777 /usr/sbin/apache2ctl

RUN echo ubuntu >> /etc/apache2/apache2.conf

CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
