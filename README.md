# First cloud native app with K8s

> Comands

```shell
kubectl create namespace kapps
```

```shell
kubectl create role poddepl --resource pod,deployment --verb list
```

```shell
kubectl create rolebinding poddepl --role poddepl --serviceaccount kapps:kapps
```

```shell
kubectl create -f app.yml -n kapps
```