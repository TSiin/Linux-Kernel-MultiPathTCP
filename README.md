# Linux-Kernel-MultiPathTCP
MPTCP

# 测试

正在测试ing...


```
grep MPTCP /boot/config-<version>
```

返回

```shell
CONFIG_MPTCP=y
CONFIG_INET_MPTCP_DIAG=m
CONFIG_MPTCP_IPV6=y
```

```
sysctl net.mptcp.enabled
```

返回

```
net.mptcp.enabled = 1
```

检查内核有没有开启MPTCP协议

```
sysctl -a | grep mptcp
```

返回

```
net.ipv4.tcp_available_ulp = espintcp mptcp tls
net.mptcp.add_addr_timeout = 120
net.mptcp.allow_join_initial_addr_port = 1
net.mptcp.checksum_enabled = 0
net.mptcp.enabled = 1
net.mptcp.pm_type = 0
net.mptcp.scheduler = default
net.mptcp.stale_loss_cnt = 4
```

如何使用 MPTCP？
https://github.com/multipath-tcp/mptcp_net-next/wiki#how-to-use-mptcp
