Note: In longhorn-servicemonitor.yaml make sure to set metadata.labels.release to what you have named the helm chart release for kube-prometheus-stack.


In the .yaml file for the service monitor, it is set to "prom" but needs to be changes.


To check the release name run the command:    helm list -A


LongHorn's official grafana dashboard can be used to test if the configuration worked https://grafana.com/grafana/dashboards/13032



To import .json file:
  1. In grafana locate and hover over the dashboard icon (a square broken up into 4 squares) on the lefthand sidebar
  2. Click the import button
  3. upload JSON file or paste contents of the file into the field below
