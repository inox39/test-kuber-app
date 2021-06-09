# test-kuber-app

## How to get repo

git clone --recursive https://github.com/inox39/test-kuber-app.git

---

## How to build

- you should use your repository
- in this example I used my public dockerhub repository

```bash
cd docker-app
docker build . -t inox39/ruby-server:v1.0
docker push inox39/ruby-server:v1.0
```

---

## How to deploy to kubernetes

```bash
cd kube-manifest
kubectl apply -f deploy-app.yml
```
