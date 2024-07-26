FROM ubuntu:24.04
COPY my-cron-job /etc/cron.d/my-cron-job
RUN chmod 644 /etc/cron.d/my-cron-job
RUN apt update
RUN apt install -y cron
RUN apt install -y sendemail
RUN apt install -y libio-socket-ssl-perl
ENTRYPOINT printenv > /etc/environment && cron -f