### About
This tutorial shows how to export kubearmor telemetry data to grafana using the kubearmor receiver and [loki exporter](https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/exporter/lokiexporter)

### Steps
1. Deploy KubeArmor
Follow [this tutorial](https://github.com/kubearmor/KubeArmor/blob/ce18fee4f87be7786dc1275aeb94ab7096c8b590/getting-started/deployment_guide.md#L20-L19) to set up KubeArmor
2. Deploy Custom Collector
- [Tutorial for k8 deployment](./tutorial.md#kubeamor-on-kubernetes-environment)
- [Tutorial  for bare metal deployment](./tutorial.md#kubeamor-on-bare-metal)
 
Note:
- Use this as [reference](https://grafana.com/docs/opentelemetry/collector/send-logs-to-loki/) for setting up collector configuration for loki exporter.
- Replace loki endpoint with your own endpoint.
- If you followed the grafana loki tutorial referenced above, you might have to, run a `docker inspect <network name used in docker compose file>` to get the endpoint.



![image](https://user-images.githubusercontent.com/59079323/235289951-6842da6f-a020-4723-81f6-02bae0987d1c.png)
