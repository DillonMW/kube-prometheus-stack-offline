Files used for offline installation of kube-prometheus-stack (community helm chart project for launching prometheus and grafana) 

The projects community pages:

  https://github.com/prometheus-community/helm-charts
  
  https://artifacthub.io/packages/helm/prometheus-community/kube-prometheus-stack


Clone prometheus helm-charts (https://github.com/prometheus-community/helm-charts) to your local machine.

The only needed directories from this repo should be kube-prometheus-stack, kube-state-metrics, prometheus-node-exporter, but it is safe to clone all of the helm charts.


Clone grafana helm-charts (https://github.com/grafana/helm-charts) to your local machine in the same location as the prometheus helm charts.

The only needed directory should be grafana, but the Chart file in kube-prometheus-stack is configured from cloning this entire repository and renamed to grafana-helm-charts.


The file pull.txt has all of the docker commands for images that need to be pulled down into a local repository to be used in the values.yaml files.


If any changes are made to files outside of kube-prometheus-stack, run the commands:

  Helm dependency run
  Helm dep update

To install run:

  Helm install name kube-prometheus-stack/ -n namespace


