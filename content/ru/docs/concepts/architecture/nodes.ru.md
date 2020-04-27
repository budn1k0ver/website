---
title: Узлы
content_template: templates/concept
weight: 10
---

{{% capture overview %}}

Узел (Node) - это VM или физический компьютер, который служит как рабочая машина в кластере Kubernetes. Каждый узел в кластере включает в себя сервисы для запуска [подов](/docs/concepts/workloads/pods/pod/), такие как [container runtime](/docs/concepts/overview/components/#container-runtime), [kubelet](docs/reference/command-line-tools-reference/kubelet/) и [kube-proxy](https://kubernetes.io/docs/reference/command-line-tools-reference/kube-proxy/).
Для более подробной информации смотри раздел архитектурного дизайна
[The Kubernetes Node](https://git.k8s.io/community/contributors/design-proposals/architecture/architecture.md#the-kubernetes-node).

{{% /capture %}}

{{% capture body %}}

## Информация о состоянии узла

Подробную информацию о состоянии узла(IP адреса, доступное пространство, CPU, вресия OS и тд) можно получить с помощью команды
```shell
kubectl describe node <insert-node-name-here>
```
или
```shell
kubectl describe nodes
```
Вся информация поделена на разделы:

* [Addresses](#addresses)
* [Conditions](#condition)
* [Capacity и Allocatable](#capacity)
* [System Info](#info)

Далее каждый раздел расмотрен более детально.

### Addresses

В разделе `Addresses` находится информация о адресах по которым доступен узел:

* `HostName`: Имя хоста. Может быть перезаписано с помощью kubelet параметра `--hostname-override`. 
* `ExternalIP`: IP адрес, по которому узел доступен извне кластера.
* `InternalIP`: IP адрес, по которому узел доступен внутри кластера.

### Conditions
### Capacity и Allocatable {#capacity}
### System Info {#info}

{{% /capture %}}