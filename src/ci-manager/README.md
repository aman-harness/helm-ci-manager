# ci-manager

![Version: 0.2.27](https://img.shields.io/badge/Version-0.2.27-informational?style=flat-square) ![Type: application](https://img.shields.io/badge/Type-application-informational?style=flat-square) ![AppVersion: 0.0.1](https://img.shields.io/badge/AppVersion-0.0.1-informational?style=flat-square)

A Helm chart for Kubernetes

## Requirements

| Repository | Name | Version |
|------------|------|---------|
| https://harness.github.io/helm-common | harness-common | 1.x.x |

## Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| affinity | object | `{}` |  |
| appLogLevel | string | `"INFO"` |  |
| autoscaling.enabled | bool | `false` |  |
| autoscaling.maxReplicas | int | `100` |  |
| autoscaling.minReplicas | int | `1` |  |
| autoscaling.targetCPUUtilizationPercentage | int | `80` |  |
| ci_images.addon.image.digest | string | `""` |  |
| ci_images.addon.image.imagePullSecrets | list | `[]` |  |
| ci_images.addon.image.registry | string | `"docker.io"` |  |
| ci_images.addon.image.repository | string | `"harness/ci-addon"` |  |
| ci_images.addon.image.tag | string | `"1.16.1-linux-amd64"` |  |
| ci_images.artifactory_upload.image.digest | string | `""` |  |
| ci_images.artifactory_upload.image.imagePullSecrets | list | `[]` |  |
| ci_images.artifactory_upload.image.registry | string | `"docker.io"` |  |
| ci_images.artifactory_upload.image.repository | string | `"plugins/artifactory"` |  |
| ci_images.artifactory_upload.image.tag | string | `"1.2.0"` |  |
| ci_images.gcs_cache.image.digest | string | `""` |  |
| ci_images.gcs_cache.image.imagePullSecrets | list | `[]` |  |
| ci_images.gcs_cache.image.registry | string | `"docker.io"` |  |
| ci_images.gcs_cache.image.repository | string | `"plugins/cache"` |  |
| ci_images.gcs_cache.image.tag | string | `"1.4.3"` |  |
| ci_images.gcs_upload.image.digest | string | `""` |  |
| ci_images.gcs_upload.image.imagePullSecrets | list | `[]` |  |
| ci_images.gcs_upload.image.registry | string | `"docker.io"` |  |
| ci_images.gcs_upload.image.repository | string | `"plugins/gcs"` |  |
| ci_images.gcs_upload.image.tag | string | `"1.3.0"` |  |
| ci_images.git_clone.image.digest | string | `""` |  |
| ci_images.git_clone.image.imagePullSecrets | list | `[]` |  |
| ci_images.git_clone.image.registry | string | `"docker.io"` |  |
| ci_images.git_clone.image.repository | string | `"harness/drone-git"` |  |
| ci_images.git_clone.image.tag | string | `"1.2.7-rootless"` |  |
| ci_images.kaniko.image.digest | string | `""` |  |
| ci_images.kaniko.image.imagePullSecrets | list | `[]` |  |
| ci_images.kaniko.image.registry | string | `"docker.io"` |  |
| ci_images.kaniko.image.repository | string | `"plugins/kaniko"` |  |
| ci_images.kaniko.image.tag | string | `"1.6.6"` |  |
| ci_images.kaniko_ecr.image.digest | string | `""` |  |
| ci_images.kaniko_ecr.image.imagePullSecrets | list | `[]` |  |
| ci_images.kaniko_ecr.image.registry | string | `"docker.io"` |  |
| ci_images.kaniko_ecr.image.repository | string | `"plugins/kaniko-ecr"` |  |
| ci_images.kaniko_ecr.image.tag | string | `"1.6.6"` |  |
| ci_images.kaniko_gcr.image.digest | string | `""` |  |
| ci_images.kaniko_gcr.image.imagePullSecrets | list | `[]` |  |
| ci_images.kaniko_gcr.image.registry | string | `"docker.io"` |  |
| ci_images.kaniko_gcr.image.repository | string | `"plugins/kaniko-gcr"` |  |
| ci_images.kaniko_gcr.image.tag | string | `"1.6.6"` |  |
| ci_images.lite_engine.image.digest | string | `""` |  |
| ci_images.lite_engine.image.imagePullSecrets | list | `[]` |  |
| ci_images.lite_engine.image.registry | string | `"docker.io"` |  |
| ci_images.lite_engine.image.repository | string | `"harness/ci-lite-engine"` |  |
| ci_images.lite_engine.image.tag | string | `"1.16.1-linux-amd64"` |  |
| ci_images.s3_cache.image.digest | string | `""` |  |
| ci_images.s3_cache.image.imagePullSecrets | list | `[]` |  |
| ci_images.s3_cache.image.registry | string | `"docker.io"` |  |
| ci_images.s3_cache.image.repository | string | `"plugins/cache"` |  |
| ci_images.s3_cache.image.tag | string | `"1.4.3"` |  |
| ci_images.s3_upload.image.digest | string | `""` |  |
| ci_images.s3_upload.image.imagePullSecrets | list | `[]` |  |
| ci_images.s3_upload.image.registry | string | `"docker.io"` |  |
| ci_images.s3_upload.image.repository | string | `"plugins/s3"` |  |
| ci_images.s3_upload.image.tag | string | `"1.1.0"` |  |
| fullnameOverride | string | `""` |  |
| global.airgap | bool | `false` |  |
| global.imagePullSecrets | list | `[]` |  |
| global.loadbalancerURL | string | `""` |  |
| image.digest | string | `""` |  |
| image.imagePullSecrets | list | `[]` |  |
| image.pullPolicy | string | `"IfNotPresent"` |  |
| image.registry | string | `"docker.io"` |  |
| image.repository | string | `"harness/ci-manager-signed"` |  |
| image.tag | string | `"2803"` |  |
| java.memory | int | `4096` |  |
| maxSurge | int | `1` |  |
| maxUnavailable | int | `0` |  |
| mongoSecrets.password.key | string | `"mongodb-root-password"` |  |
| mongoSecrets.password.name | string | `"mongodb-replicaset-chart"` |  |
| mongoSecrets.userName.key | string | `"mongodbUsername"` |  |
| mongoSecrets.userName.name | string | `"harness-secrets"` |  |
| nameOverride | string | `""` |  |
| nodeSelector | object | `{}` |  |
| podAnnotations | object | `{}` |  |
| podSecurityContext | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources.limits.cpu | int | `1` |  |
| resources.limits.memory | string | `"8192Mi"` |  |
| resources.requests.cpu | int | `1` |  |
| resources.requests.memory | string | `"1400Mi"` |  |
| securityContext.runAsNonRoot | bool | `true` |  |
| securityContext.runAsUser | int | `65534` |  |
| securityImage.image.digest | string | `""` |  |
| securityImage.image.imagePullSecrets | list | `[]` |  |
| securityImage.image.registry | string | `"docker.io"` |  |
| securityImage.image.repository | string | `"harness/sto-plugin"` |  |
| securityImage.image.tag | string | `"latest"` |  |
| service.grpcport | int | `9979` |  |
| service.port | int | `7090` |  |
| service.type | string | `"ClusterIP"` |  |
| serviceAccount.annotations | object | `{}` |  |
| serviceAccount.create | bool | `false` |  |
| serviceAccount.name | string | `"harness-default"` |  |
| stoServiceGlobalToken.key | string | `"stoAppHarnessToken"` |  |
| stoServiceGlobalToken.name | string | `"harness-secrets"` |  |
| timescaleSecret.password.key | string | `"timescaledbPostgresPassword"` |  |
| timescaleSecret.password.name | string | `"harness-secrets"` |  |
| tolerations | list | `[]` |  |
| waitForInitContainer.image.digest | string | `""` |  |
| waitForInitContainer.image.imagePullSecrets | list | `[]` |  |
| waitForInitContainer.image.pullPolicy | string | `"IfNotPresent"` |  |
| waitForInitContainer.image.registry | string | `"docker.io"` |  |
| waitForInitContainer.image.repository | string | `"harness/helm-init-container"` |  |
| waitForInitContainer.image.tag | string | `"latest"` |  |

