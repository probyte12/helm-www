+++
title = "helm inspect"
weight = "17"

tags = ["commands"]
section = "helm-commands"
categories = ["helm-commands"]
type = "page"

slug = "helm-inspect"

[menu.main]
  url = "helm-inspect"
  parent = "helm-commands"

+++

## helm inspect

inspect a chart

### Synopsis



This command inspects a chart and displays information. It takes a chart reference
('stable/drupal'), a full path to a directory or packaged chart, or a URL.

Inspect prints the contents of the Chart.yaml file and the values.yaml file.


```
helm inspect [CHART]
```

### Options

```
      --ca-file string     chart repository url where to locate the requested chart
      --cert-file string   verify certificates of HTTPS-enabled servers using this CA bundle
      --key-file string    identify HTTPS client using this SSL key file
      --keyring string     path to the keyring containing public verification keys (default "~/.gnupg/pubring.gpg")
      --repo string        chart repository url where to locate the requested chart
      --verify             verify the provenance data for this chart
      --version string     version of the chart. By default, the newest chart is shown
```

### Options inherited from parent commands

```
      --debug                     enable verbose output
      --home string               location of your Helm config. Overrides $HELM_HOME (default "~/.helm")
      --host string               address of tiller. Overrides $HELM_HOST
      --kube-context string       name of the kubeconfig context to use
      --tiller-namespace string   namespace of tiller (default "kube-system")
```

### SEE ALSO
* [helm](#helm)	 - The Helm package manager for Kubernetes.
* [helm inspect chart](#helm-inspect-chart)	 - shows inspect chart
* [helm inspect values](#helm-inspect-values)	 - shows inspect values
