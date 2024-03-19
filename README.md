# cilium

spec:
  patches:
    - patch: |-
        apiVersion: apps/v1
        kind: Pod
        metadata:
          name: guestbook
        spec:
          replicas: 2             
      target:
        name: guestbook
        kind: Pod