FROM ubuntu:16.04

RUN apt-get update && apt-get install -y cron rsyslog

COPY task_cron /etc/cron.d/

RUN mkdir /data

CMD service rsyslog start && service cron start && tail -f /var/log/syslog