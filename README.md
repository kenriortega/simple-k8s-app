# First cloud native app with K8s

> Comands

```shell
kubectl create role poddepl --resource pod,deployment --verb list
```

```shell
kubectl create rolebinding poddepl --role poddepl --serviceaccount default:default
```

```shell
kubectl create -f app.yml
```