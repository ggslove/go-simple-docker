
#  syscall 在docker中的应用

| Namespace | 调用参数 | 用途 |
| :--- | :--- | :---|
| Mount | CLONE_NEWNS| 隔离文件系统挂载点，容器内的挂载操作不影响宿主机和其他容器 |
| UTS   | CLONE_NEWUTS| 隔离主机名和域名，让容器拥有独立的主机标识 |
| IPC   | CLONE_NEWIPC | 隔离进程间通信资源（如信号量、消息队列、共享内存）|
| PID   | CLONE_NEWPID | 隔离进程 ID 空间，容器内 PID 从 1 开始，与宿主机互不干扰 |
| Network | CLONE_NEWNET | 隔离网络资源，包括网卡、IP 地址、端口、路由表、防火墙规则等 |
| User | CLONE_NEWUSER| 隔离用户和用户组 ID，实现容器内普通用户映射为宿主机特权用户（或反之）|
| Cgroup | CLONE_NEWCGROUP | 隔离 cgroup 根目录，让容器拥有独立的 cgroup 资源管理视图 |

