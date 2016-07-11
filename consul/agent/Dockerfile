#
# Starts a consul agent
#
FROM lycis/consul

VOLUME ["/tmp/"]
VOLUME ["/etc/consul/"]

# server, lan, wan serf
EXPOSE 8300-8302
# rpc
EXPOSE 8400
# http
EXPOSE 8500
# dns
EXPOSE 8600

CMD ["agent", "-data-dir", "/tmp/", "-config-dir", "/etc/consul/"]
