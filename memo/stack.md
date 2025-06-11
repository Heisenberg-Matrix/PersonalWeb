# 交换机堆叠Stack配置



## 配置



```
主交换机：
#
  interface stack-port 0/1
  port interface XGigabitEthernet 0/0/3 enable
  #
  int stack-port 0/2
  port interface XGigabitEthernet 0/0/4 enable
  #
 stack slot 0 priority 200
  
备交换机：
 interface stack-port 0/1
  port interface XGigabitEthernet 0/0/3 enable
  #
  int stack-port 0/2
  port interface XGigabitEthernet 0/0/4 enable
  #
stack slot 0 renumber 1
```



MAD多主监测

```
int g0/0/48 （二层端口）
mad detect mode direct
stp disable
```



## 查看









Last update: 2025-06