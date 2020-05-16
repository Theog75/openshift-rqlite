# rqlite for Openshift /Kubernetes

This deployment will run a 3 cluster (or more - configurable at the number of replicas in the statefulset) of [rqlite](https://github.com/rqlite/rqlite) distributed in-memory sqlite database.

This will provide a highly available sqlite database which runs perfectly on Openshift (and Kubernetes in general).

## Quick setup

Simply clone this repository and run:

**On Kubernetes**
```
kubectl apply -f rqlite.yml
```

**On Openshift**
```
oc apply -f rqlite.yml
```

This will create the Pods in running rqlite and the service required for their internat communication.

For more information about rqlite click [here](https://github.com/rqlite/rqlite)