# Valkey Backup Helm Chart

- [License](https://www.apache.org/licenses/LICENSE-2.0.txt)
- [Release](https://github.com/andinod/valkey-backup-helm/releases)

## Introduction

This helm chart is intended to create a Job or a Cronjob for Valkey instances that are based on the Bitnami's Valkey. The Job or the Cronjob will save the redis dump file into a Generic S3. 

Theorically it can also support GCP, AWS and AZURE, but these are not tested.

## Features

- Helm Chart to make the backup of the valkey instance into S3

## Installation

### Prerequisites

- Kubernetes v1.32.0+
- Helm

### Using Helm

Deploy using Helm (version 3.8.0 or later). In the following link you will get the proper instructions [Helm Installation](https://andinod.github.io/valkey-backup-helm/).

```bash
helm upgrade --install valkey-standalone-instance https://andinod.github.io/valkey-backup-helm/charts/valkey-backup -f myvalues.yaml
```

Please set the customized values in a file based on the values.yaml file of the Chart.


## Contributing

Contributions are warmly welcomed. Feel free to submit issues or pull requests.

## Links used for construction

As an additional information is added the list of links for documentation and instructions:

- [Bitnami Valkey](https://artifacthub.io/packages/helm/bitnami/valkey)
- [Helm Operator Tutorial](https://sdk.operatorframework.io/docs/building-operators/helm/tutorial/)

## License

This project is licensed under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0.txt).
