# gateway-local-env

# Grafana

```shell
docker run -d -p 3000:3000 grafana/grafana-oss
```

admin/admin

# Prometheus

```shell
docker run \                                                                                                                                          ✔  34s  18:13:39 
    -p 9090:9090 \
    -v /Users/scaat/Projects/Java/gw/prometheus/prometheus.yml:/etc/prometheus/prometheus.yml \
    prom/prometheus
```

# Sentinel Dashboard

```shell
mvn clean package
```

```shell
java -Dserver.port=8080 \
-Dcsp.sentinel.dashboard.server=localhost:8080 \
-Dproject.name=sentinel-dashboard \
-jar target/sentinel-dashboard.jar
```

sentinel/sentinel

# Apollo

```shell
docker-compose up
```

apollo/admin
