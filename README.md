# pmm-workshop

```bash
docker-compose up pmm-server
```

```bash
docker-compose up pmm-client
```

```bash
docker exec -it pmm-client pmm-admin inventory add node generic --address=host.docker.internal host
```

```bash
docker exec -it pmm-client pmm-admin add external --listen-port=9100 --service-name=workshop --service-node-id=<HOST NODE ID> --agent-node-id=<HOST NODE ID> --metrics-path=/prom
```

http://127.0.0.1/graph/d/pmm-inventory/pmm-inventory

http://127.0.0.1/prometheus/targets

http://127.0.0.1/graph/d/prometheus-advanced/advanced-data-exploration
