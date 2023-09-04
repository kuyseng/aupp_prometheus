- Copy default `prometheus.yml` file.

```bash
docker run --rm --entrypoint cat prom/prometheus /etc/prometheus/prometheus.yml > prometheus.yml
```

 docker run \
  --volume=/:/rootfs:ro \
  --volume=/var/run:/var/run:rw \
  --volume=/sys:/sys:ro \
  --volume=/var/lib/docker/:/var/lib/docker:ro \
  --publish=8080:8080 \
  --detach=true \
  --name=cadvisor \

### Refs
- https://stackoverflow.com/questions/25292198/docker-how-can-i-copy-a-file-from-an-image-to-a-host
- https://prometheus.io/docs/guides/cadvisor/
- https://hub.docker.com/r/raymondmm/cadvisor
- https://hub.docker.com/r/zcube/cadvisor
- https://grafana.com/grafana/dashboards/14282-cadvisor-exporter/

- https://github.com/google/cadvisor/issues/1565