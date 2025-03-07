## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

```shell
helm repo add andinod-backup https://andinod.github.io/valkey-backup-helm
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
andinod` to see the charts.

Please refer to the values.yaml file to provide the required parameters.

To install the valkey-backup chart:

    helm upgrade --install backup-standalone andinod-backup/valkey-backup -f myvalues.yaml

To uninstall the chart:

    helm uninstall backup-standalone

