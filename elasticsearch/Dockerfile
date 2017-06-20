# https://github.com/elastic/elasticsearch-docker
FROM docker.elastic.co/elasticsearch/elasticsearch:5.2.2
USER root
RUN apk update
RUN apk upgrade
# Change TimeZone
RUN apk add --update tzdata
ENV TZ=Europe/Paris

USER elasticsearch
CMD ["/bin/bash", "bin/es-docker"]

EXPOSE 9200 9300