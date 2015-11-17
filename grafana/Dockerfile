#
# Stock Grafana + a few custom dashboards
#

FROM grafana/grafana

RUN apt-get update && \
    apt-get install -y curl

COPY dashboards /dashboards
COPY run.sh /run.sh
COPY conf /conf

EXPOSE 3000
ENTRYPOINT /run.sh
