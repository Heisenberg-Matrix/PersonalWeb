

公司有这样一个需求：用户跨办公点搬迁后，保持IP不变。

一般来说，路由器互联的不同办公地点的用户IP网段肯定不一样。因为需要配置不同的路由连通各个分部。如果网段混杂在一起，管理和变更成本就会极高。

但是仔细一想，其实 VLAN 的思想可以解决这个问题：



也就是说，需求的导向会使网络向着与物理解耦的方向发展。更加灵活、多变、可扩展。

最早的时候VLAN 让物理网络拓扑和逻辑网络拓扑能够分开，比如1楼的用户可以是财务，行政，而不用都坐在同一栋楼共享一个



以H3C S7503X为例介绍VXLAN配置



两边Loopback IP回环地址 10.0.0.1 ，10.0.0.2

建立一个tunnel 端口

