# Kubernetes external-storage NFS provisioner

A Helm chart for dynamic NFS persistent volumes based on https://github.com/kubernetes-incubator/external-storage/blob/233b44b89dee15d9ec4ba2e084abb74735a60909/nfs/deploy/kubernetes

You must either either create a PersistentVolumeClaim such as [`pvc-kubespray-glusterfs.yaml`](pvc-kubespray-glusterfs.yaml) to back the dynamically created NFS volumes , or specify a hostPath.

This chart defaults to creating `StorageClass: external-storage-nfs-provisioner`.
