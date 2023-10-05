- helm dependency build
- helm upgrade --install release-name  ../helm-universal/ -f test.yaml 

and dont forget create this file:
```
apiVersion: v1
kind: Secret
metadata:
  name: registry-secret
  namespace: default
type: kubernetes.io/dockerconfigjson
data:
  .dockerconfigjson: >-
    some_shitty_text_here
```
