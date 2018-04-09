# influxdb-grafana-docker
Docker Compose recipe for Influx DB and Grafana

##### Startup
```
docker-compose up -d
```

##### Shutdown
```
docker-compose down
```

##### CLI
Connect to the influx db via cli:
```
docker run --rm --link=influxdbgrafanadocker_influxdb_1 -it --net influxdbgrafanadocker_influx-net influxdb influx -host influxdbgrafanadocker_influxdb_1
```
