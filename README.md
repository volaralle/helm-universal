- helm dependency build
- helm upgrade --install aaa  ../helm-universal/ -f test.yaml 

+
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
