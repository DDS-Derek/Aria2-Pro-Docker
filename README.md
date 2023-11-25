# Aria2 Pro Docker

根据 https://github.com/P3TERX/Aria2-Pro-Docker 大佬镜像改编

1. Add `DOWNLOAD_DIR` environment variables
2. 自动 ban 掉迅雷等不受欢迎客户端，**`NET_ADMIN` 对于 ipset 是必需的**
```yaml
...
    cap_add:
      - NET_ADMIN
...
```
3. Anime trackers
```shell
https://raw.githubusercontent.com/DDS-Derek/Aria2-Pro-Docker/main/tracker/all.list
https://ddsrem.com/alltracker
https://raw.dov.moe/DDS-Derek/Aria2-Pro-Docker/main/tracker/all.list
```