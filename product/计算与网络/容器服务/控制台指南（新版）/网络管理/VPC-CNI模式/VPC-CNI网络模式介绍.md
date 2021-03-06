

VPC-CNI 模式是容器服务 TKE 基于 CNI 和 VPC 弹性网卡实现的容器网络能力，适用于对时延有较高要求的场景。该网络模式下，容器与节点分布在同一网络平面，容器 IP 为 IPAMD 组件所分配的弹性网卡 IP。

其中 VPC-CNI 模式分为共享网卡模式和独占网卡模式。两种网络模式适用于不同的场景。您可以根据业务需要选择不同的网络模式。
- [共享网卡模式](https://cloud.tencent.com/document/product/457/50356)：Pod 共享一张弹性网卡，IPAMD 组件为弹性网卡申请多个 IP 给到不同的 Pod。
- [独占网卡模式](https://cloud.tencent.com/document/product/457/50357)：每个 Pod 有独立的弹性网卡，性能更高。受机型影响，不同节点可使用的弹性网卡数量有限，单节点 Pod 密度更低。



