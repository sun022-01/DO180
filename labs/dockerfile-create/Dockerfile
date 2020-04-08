FROM ubi7/ubi:7.7
ENV PORT=8080
MAINTAINER Your Name nicolas.m.aguero.e@set.ypf.com
LABEL description="A basic Apache container on RHEL 7 UBI"
RUN yum install -y httpd && \
yum clean all
RUN echo "Hello from Docerfile" > /usr/share/httpd/noindex/index.html
EXPOSE 80
ENTRYPOINT ["httpd", "-D", "FOREGROUND"]
