# Holt（profile-v1 WordPress 子站）

明日方舟 / 音乐作品集主题站，挂载为主题目录名 `holt-portfolio`。

- 公网：`/wp/holt/`
- 父仓：`profile-v1` 以 submodule 路径 `wordpress/holt` 集成
- 主题目录即本仓根目录（`style.css` / `functions.php` …）
- 作品种子数据：`data/holt-bilibili-works.json`

## 本地（父仓）

```bash
git submodule update --init wordpress/holt
# 网关：deploy/docker-compose.gateway.yml 挂载 ../wordpress/holt → themes/holt-portfolio
# 或：cd deploy/wordpress && docker compose -f docker-compose.dev.yml up -d
```
