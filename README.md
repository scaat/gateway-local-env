# gateway-local-env

# Grafana

```shell
docker run -d -p 3000:3000 grafana/grafana-oss
```

admin/admin

# Prometheus

```shell
docker run -d \
    -p 9090:9090 \
    -v /Users/scaat/Projects/Java/gw/prometheus/prometheus.yml:/etc/prometheus/prometheus.yml \
    prom/prometheus
```

# Sentinel Dashboard

```shell
mvn -f Sentinel-1.8.6/sentinel-dashboard/pom.xml clean package
```

```shell
java -Dserver.port=8088 \
-Dcsp.sentinel.dashboard.server=localhost:8088 \
-Dproject.name=sentinel-dashboard \
-jar Sentinel-1.8.6/sentinel-dashboard/target/sentinel-dashboard.jar
```

sentinel/sentinel

# Apollo

```shell
docker-compose up
```

apollo/admin

# Consul

```shell

```
