# Simple WebApp Helm Chart
This is a Helm Chart for learning purpos

**Installation**
First clone this repository to your local machine:
```
git clone https://github.com/aa-shoja/simple-webapp-helm
```
Then install the chart with:
```
helm install myapp .
```

##Configuration
The following table list the configurable parameters and their default values:

| Parameter | Description | Default |
| --- | --- | --- |
| `image.repository` | Docker image repository | `amashk/simple-webapp-python-alpine` |
| `image.tag` | Docker image tag | `v1` |
| `service.type` | Kubernetes service type | `NodePort` |
| `service.port` | Kubernetes service port | `5000` |
| `ingress.enabled` | Enable ingress | `false` |
| `ingress.hosts` | Ingress hostnames | `[]` |
| `ingress.annotations` | Ingress annotations | `{}` |

Specify each parameter using the **'--set key=value[,key=value]'** argument to **'helm install'**

To access the node, point your browser to the `http://<nodeIP>:30072/status`
