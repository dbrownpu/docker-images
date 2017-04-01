FROM debian:jessie

RUN apt-get update && apt-get install -y mosquitto mosquitto-clients && apt-get clean

LABEL org.freenas.interactive="false"			\
      org.freenas.version="1"				\
      org.freenas.upgradeable="true"			\
      org.freenas.expose-ports-at-host="true"		\
      org.freenas.autostart="true"			\
      org.freenas.port-mappings="8083:8083/tcp"		\
      
EXPOSE 8083

ENTRYPOINT ["/usr/sbin/mosquitto"]              
