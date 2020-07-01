Example - Kaniko build and push image to Docker hub

Environment - Window Wsl2, Kubernetes cluster(kind) with 3 nodes, Kaniko and Docker hub

Create dockerfile in respective node

Copy Docker's config.json to respective node

Create secret

kubectl create secret generic docker-secret --from-file=./config.json

Change docker repo in pod.yaml

https://www.baeldung.com/ops/kaniko

https://github.com/GoogleContainerTools/kaniko/issues/835
