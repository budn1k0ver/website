---
title: Узлы
content_template: templates/concept
weight: 10
---

{{% capture overview %}}

Узел (Node) - это VM или физический компьютер, который служит как рабочая машина в кластере Kubernetes. Каждый узел в кластере Kubernetes включает в себя сервисы для запуска [подов](/docs/concepts/workloads/pods/pod/), такие как [container runtime](/docs/concepts/overview/components/#container-runtime), [kubelet](docs/reference/command-line-tools-reference/kubelet/) и [kube-proxy](https://kubernetes.io/docs/reference/command-line-tools-reference/kube-proxy/).
Для более подробной информации смотри раздел архитектурного дизайна
[The Kubernetes Node](https://git.k8s.io/community/contributors/design-proposals/architecture/architecture.md#the-kubernetes-node).

{{% /capture %}}

{{% capture body %}}

## Статус узла

Статус узла содержит следующую ифнормацию:

* [Адреса](#addresses)
* [Состояния](#condition)
* [Доступная емкость](#capacity)
* [Информация](#info)

Node status and other details about a node can be displayed using the following command:
```shell
kubectl describe node <insert-node-name-here>
```
Each section is described in detail below.

### Адреса {#addresses}
### Состояния {#condition}
### Доступная емкость {#capacity}
### Информация

{{% /capture %}}