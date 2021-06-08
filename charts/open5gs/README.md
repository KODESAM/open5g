# open5gs

![Version: 0.1.2](https://img.shields.io/badge/Version-0.1.2-informational?style=flat-square) ![AppVersion: 2.2.3](https://img.shields.io/badge/AppVersion-2.2.3-informational?style=flat-square)

Helm chart to deploy Open5gs services on Kubernetes.

**Homepage:** <https://github.com/gradiant/openverso-charts>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| cgiraldo | cgiraldo@gradiant.org |  |

## Source Code

* <http://open5gs.org>

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://charts.bitnami.com/bitnami | mongodb | ~9.2.2 |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| amf.logger.level | string | `"info"` |  |
| amf.mcc | string | `"001"` |  |
| amf.mnc | string | `"01"` |  |
| amf.parameter | object | `{}` |  |
| amf.region | string | `"2"` |  |
| amf.resources | object | `{}` |  |
| amf.set | string | `"1"` |  |
| amf.sst | string | `"1"` |  |
| amf.tac | string | `"0001"` |  |
| ausf.logger.level | string | `"info"` |  |
| ausf.parameter | object | `{}` |  |
| ausf.resources | object | `{}` |  |
| hss.logger.level | string | `"info"` |  |
| hss.resources | object | `{}` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"openverso/open5gs"` |  |
| image.tag | string | `"2.1.7"` |  |
| mme.logger.level | string | `"info"` |  |
| mme.mcc | string | `"001"` |  |
| mme.mnc | string | `"01"` |  |
| mme.parameter | object | `{}` |  |
| mme.resources | object | `{}` |  |
| mme.tac | string | `"0001"` |  |
| mongodb | object | `{"auth":{"enabled":false},"enabled":true}` | pass vars towards mongodb chart, from dependencies |
| mongodb.enabled | bool | `true` | set to 'false' to disable automatically deploying dependent charts |
| nrf.logger.level | string | `"info"` |  |
| nrf.parameter | object | `{}` |  |
| nrf.resources | object | `{}` |  |
| pcrf.enabled | bool | `false` |  |
| pcrf.logger.level | string | `"info"` |  |
| pcrf.parameter | string | `nil` |  |
| pcrf.resources | object | `{}` |  |
| securityPolicy.enabled | bool | `false` |  |
| sgwc.logger.level | string | `"info"` |  |
| sgwc.max | object | `{}` |  |
| sgwc.parameter.no_ipv6 | bool | `true` |  |
| sgwc.pool | object | `{}` |  |
| sgwc.resources | object | `{}` |  |
| sgwu.logger.level | string | `"info"` |  |
| sgwu.max | object | `{}` |  |
| sgwu.parameter.no_ipv6 | bool | `true` |  |
| sgwu.pool | object | `{}` |  |
| sgwu.resources | object | `{}` |  |
| smf.logger.level | string | `"info"` |  |
| smf.parameter | object | `{}` |  |
| smf.pdn.addr | string | `"10.45.0.1/16"` |  |
| smf.resources | object | `{}` |  |
| udm.logger.level | string | `"info"` |  |
| udm.parameter | object | `{}` |  |
| udm.resources | object | `{}` |  |
| udr.logger.level | string | `"info"` |  |
| udr.parameter | object | `{}` |  |
| udr.resources | object | `{}` |  |
| upf.logger.level | string | `"info"` |  |
| upf.parameter | object | `{}` |  |
| upf.pdn.addr | string | `"10.45.0.1/16"` |  |
| upf.resources | object | `{}` |  |
| webui.image.pullPolicy | string | `"Always"` |  |
| webui.image.registry | string | `"docker.io"` |  |
| webui.image.repository | string | `"openverso/open5gs-webui"` |  |
| webui.image.tag | string | `"2.1.7"` |  |
| webui.ingress.annotations | object | `{}` |  |
| webui.ingress.certManager | bool | `false` |  |
| webui.ingress.enabled | bool | `false` |  |
| webui.ingress.hostname | string | `"open5gs.local"` |  |
| webui.ingress.path | string | `"/"` |  |
| webui.ingress.pathType | string | `"ImplementationSpecific"` |  |
| webui.ingress.tls | bool | `false` |  |
| webui.resources | object | `{}` |  |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)