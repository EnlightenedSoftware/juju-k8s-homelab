# juju-k8s-homelab
Trying to realize the following tutorial:
https://ubuntu.com/tutorials/how-to-build-a-ceph-backed-kubernetes-cluster#1-overview

## Issue
After deployment I get the following error:

```juju deploy ./bundle.yaml
WARNING "services" key found in bundle file is deprecated, superseded by "applications" key.
Located charm "ceph-mon" in charm-store, channel stable
Located charm "ceph-osd" in charm-store, channel stable
Located charm "containerd" in charm-store, revision 97
Located charm "easyrsa" in charm-store, revision 339
Located charm "etcd" in charm-store, revision 544
Located charm "flannel" in charm-store, revision 513
Located charm "kubeapi-load-balancer" in charm-store, revision 753
Located charm "kubernetes-master" in charm-store, revision 912
Located charm "kubernetes-worker" in charm-store, revision 713
Executing changes:
- upload charm ceph-mon from charm-store for series focal with architecture=amd64
- deploy application ceph-mon from charm-store on focal
ERROR cannot deploy bundle: cannot deploy application "ceph-mon": space not found```
