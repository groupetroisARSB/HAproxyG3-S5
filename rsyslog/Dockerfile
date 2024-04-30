FROM jumanjiman/rsyslog

# RUN apk update && apk add --no-cache rsyslog
# RUN mkdir -p /tmp/rsyslog && chmod 755 /tmp/rsyslog
# RUN chown root:root /tmp/rsyslog

RUN touch /var/log/haproxy.log
RUN chown root:root /var/log/haproxy.log
RUN chmod 777 /var/log/haproxy.log

# RUN /usr/sbin/usermod -aG root rsyslog

COPY rsyslog.conf /etc/rsyslog.conf

WORKDIR /app

EXPOSE 514

CMD ["/usr/sbin/rsyslogd", "-i", "/etc/rsyslog.conf"]

