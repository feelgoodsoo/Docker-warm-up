FROM ubuntu:14.04
LABEL maintainer "pschoi <chlvlftn22@naver.com>"
LABEL "purpose"="practice"
RUN sudo apt-get update
RUN sudo apt-get install apache2 -y
ADD test.html /var/www/html
WORKDIR /var/www/html
RUN ["/bin/bash", "-c", "echo hello >> test2.html"]
EXPOSE 80
CMD apachectl -DFOREGROUND
