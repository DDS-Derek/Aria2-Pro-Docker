# Aria2 Pro Docker

根据 https://github.com/P3TERX/Aria2-Pro-Docker 大佬镜像改编

1. 增加`DOWNLOAD_DIR`环境变量
2. 自动 ban 掉迅雷等不受欢迎客户端，**NET_ADMIN 对于 ipset 是必需的**
```
...
    cap_add:
      - NET_ADMIN
...
```
