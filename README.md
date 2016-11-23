# hacking_k8s

## Install docker k8s first

```
# ./install_k8s.sh
```

## init master controller
On Master node, run as root user
```
# kubeadm init
```
And make a record of token, such as:

```
$ kubeadm join --token=52df86.88816a5c5eae2d9c 10.0.0.16
```

## join node
On each node

```
$ kubeadm join --token=52df86.88816a5c5eae2d9c 10.0.0.16
```
