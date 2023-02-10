# promeyheus
docker-compose up -d

docker cp prometheus.yml a0017408d566:/etc/prometheus/prometheus.yml

docker kill -s SIGHUP a0017408d566

docker cp alertmanager.yml a0017408d566:/etc/alertmanager/alertmanager.yml

docker kill -s SIGHUP a0017408d566

docker cp prometheus.yml a0017408d566:/etc/prometheus/rules.yml

docker kill -s SIGHUP a0017408d566

docker cp alert.rules a0017408d566:/etc/prometheus/alert.rules


