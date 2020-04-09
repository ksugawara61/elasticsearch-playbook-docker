FROM logstash:7.6.1

LABEL maintenar "katsuya sugawara"

RUN rm -rf /usr/share/logstash/pipeline
COPY ./assets/logstash/pipeline /usr/share/logstash/pipeline
