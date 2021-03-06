# auth-server-key-rotation

![Version: 1.0.0-b7](https://img.shields.io/badge/Version-1.0.0--b7-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 1.0.0-b7](https://img.shields.io/badge/AppVersion-1.0.0--b7-informational?style=flat-square)

Responsible for regenerating auth-keys per x hours

**Homepage:** <https://jans.io>

## Maintainers

| Name | Email | Url |
| ---- | ------ | --- |
| Mohammad Abudayyeh | support@jans.io | https://github.com/moabu |

## Source Code

* <https://github.com/JanssenProject/docker-jans-certmanager>
* <https://github.com/JanssenFederation/cloud-native-edition/tree/master/pyjans/kubernetes/templates/helm/jans/charts/auth-server-key-rotation>

## Requirements

Kubernetes: `>=v1.17.0-0`

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| dnsConfig | object | `{}` | Add custom dns config |
| dnsPolicy | string | `""` | Add custom dns policy |
| image.pullPolicy | string | `"IfNotPresent"` | Image pullPolicy to use for deploying. |
| image.repository | string | `"janssenproject/certmanager"` | Image  to use for deploying. |
| image.tag | string | `"1.0.0_b7"` | Image  tag to use for deploying. |
| keysLife | int | `48` | Auth server key rotation keys life in hours |
| nodeSelector | object | `{}` |  |
| resources | object | `{"limits":{"cpu":"300m","memory":"300Mi"},"requests":{"cpu":"300m","memory":"300Mi"}}` | Resource specs. |
| tolerations | list | `[]` |  |
| usrEnvs.normal | object | `{}` | Add custom normal envs to the service variable1: value1 |
| usrEnvs.secret | object | `{}` | Add custom secret envs to the service variable1: value1 |
| volumeMounts | list | `[]` | Configure any additional volumesMounts that need to be attached to the containers |
| volumes | list | `[]` | Configure any additional volumes that need to be attached to the pod |

----------------------------------------------
Autogenerated from chart metadata using [helm-docs v1.5.0](https://github.com/norwoodj/helm-docs/releases/v1.5.0)
