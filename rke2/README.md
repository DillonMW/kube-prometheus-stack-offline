Location for this file: /ect/rancher/rke2/

NOTE: The address fields will need to be changed to your own ip address.

To allow changes to rke2, restart the rke2-server.service and they will automatically apply.

The changes are to the pod-manifests (/var/lib/rancher/rke2/agent/pod-manifests) for kube-proxy, kube-scheduler, kube-controller-manager, etcd and to etcd's config file (/var/lib/rancher/rke2/server/db/etcd/config).
