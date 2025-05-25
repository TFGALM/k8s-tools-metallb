# Instalación

```bash
 helm repo add metallb https://metallb.github.io/metallb
 #helm show values metallb/metallb --version 0.14.8 > values-default.yaml
 kubectl create namespace metallb
 helm upgrade --install metallb metallb/metallb -f values-modified.yaml --version 0.14.8 -n metallb
```