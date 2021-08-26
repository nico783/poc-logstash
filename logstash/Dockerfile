ARG ELK_VERSION

# https://www.docker.elastic.co/
FROM docker.elastic.co/logstash/logstash:${ELK_VERSION}

# Add your logstash plugins setup here
COPY mysql-connector-java-8.0.26.jar /usr/share/logstash/logstash-core/lib/jars
RUN logstash-plugin install logstash-integration-jdbc
