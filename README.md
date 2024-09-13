Old version:
https://github.com/kubernetes-retired/external-storage/tree/master/nfs-client

New Version:
https://github.com/kubernetes-sigs/nfs-subdir-external-provisioner

With Helm
Follow the instructions from the helm chart README.

```
$ helm repo add nfs-subdir-external-provisioner https://kubernetes-sigs.github.io/nfs-subdir-external-provisioner/
$ helm install nfs-subdir-external-provisioner nfs-subdir-external-provisioner/nfs-subdir-external-provisioner \
    --set nfs.server=x.x.x.x \
    --set nfs.path=/exported/path
```

