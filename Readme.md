## A home for my own helm charts
!!! This is a playground / sandbox repo !!!


### Some HELM things for me to remenber

```
$ helm create my-app
$ helm lint my-app
$ helm package my-app
$ helm install my-app my-app-0.1.x.tgz -n my-app --dry-run --debug 
$ helm repo index .  

```

Note:<br>
To push a Helm chart using the Helm CLI, first install the helm push plugin from chartmuseum/helm-push. It is not possible to push a provenance file using the Helm CLI.

E.g. Mirantis and Harbor
```
$ helm login https://...
$ helm pull <reponame>/<chartname> --version <chartversion>
$ helm push <chartname>-<chartversion>.tgz <reponame> --username <username> --password <password> --ca-file ca.crt
```