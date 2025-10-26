```yaml
apiVersion: argoproj.io/v1alpha1
kind: Application
metadata:
  name: xxx-app
  namespace: argocd
spec:
  project: default
  source:
    repoURL: https://github.com/namsic/n4c-manifests.git
    path: manifests/xxx
  destination:
    server: https://kubernetes.default.svc
    namespace: xxx
```
