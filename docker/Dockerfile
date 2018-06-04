FROM openjdk:8u151-jre-alpine3.7
MAINTAINER Andrey Kozichev <akozichev@gmail.com>
ENV COLLECTOR_HOME /opt/skywalking/collector/
ENV JAVA_OPTS=" -Xms256M -Xmx512M"
RUN mkdir -p /opt/skywalking/collector/config
COPY collector-libs/ /opt/skywalking/collector/collector-libs
CMD /usr/bin/java  -Xms256M -Xmx512M -cp "/opt/skywalking/collector/collector-libs/*:/opt/skywalking/collector/config" org.apache.skywalking.apm.collector.boot.CollectorBootStartUp

