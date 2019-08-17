http-echo
=========
http-echo is an in-memory web server that renders an HTML page containing the
contents of the arguments provided to it. This is especially useful for demos or
a more extensive "hello world" Docker application.

Current chart version is `0.1.0`

## Chart Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| fullnameOverride | string | `""` |  |
| httpEcho.listenPort | int | `5678` |  |
| httpEcho.text | string | `"hello world"` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.repository | string | `"hashicorp/http-echo"` |  |
| image.tag | string | `"0.2.3"` |  |
| imagePullSecrets | list | `[]` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0].host | string | `"chart-example.local"` |  |
| ingress.hosts[0].paths | list | `[]` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| service.port | int | `80` |  |
| service.type | string | `"ClusterIP"` |  |
| tolerations | list | `[]` |  |
