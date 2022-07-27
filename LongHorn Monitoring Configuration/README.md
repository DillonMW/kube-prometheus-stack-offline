Note: Make sure to set metadata.labels.release to what you have named the helm chart release for kube-prometheus-stack.


In the .yaml file for the service monitor, it is set to "prom" but needs to be changes.


To check the release name run the command:    helm list -A
