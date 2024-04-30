FROM haproxy:latest

# RUN mkdir -p /var/run && chmod 660 /var/run/api.sock

COPY ./haproxy.cfg /etc/haproxy/haproxy.cfg

CMD ["haproxy", "-f", "/etc/haproxy/haproxy.cfg"]