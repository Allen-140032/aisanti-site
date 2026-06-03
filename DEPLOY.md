# aisanti.site 部署说明

## 目标仓库

建议仓库：

```text
https://github.com/Allen-140032/aisanti-site
```

当前本地仓库已设置远程：

```text
origin https://github.com/Allen-140032/aisanti-site.git
```

## GitHub Pages 设置

1. 在 GitHub 创建空仓库 `aisanti-site`。
2. 推送本地仓库：

```powershell
git push -u origin main
```

3. 打开仓库 `Settings -> Pages`。
4. Source 选择：

```text
Deploy from a branch
Branch: main
Folder: / (root)
```

5. Custom domain 填：

```text
aisanti.site
```

仓库根目录已包含 `CNAME`：

```text
aisanti.site
```

## DNS 配置

裸域名 `aisanti.site` 配置 GitHub Pages 官方 A 记录：

```text
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

建议同时添加 `www`：

```text
类型：CNAME
主机记录：www
记录值：Allen-140032.github.io
```

## 验收

1. GitHub Pages 临时地址可访问。
2. `https://aisanti.site` 可访问。
3. GitHub Pages 中 `Enforce HTTPS` 可开启。
4. 页面检查：
   - `/`
   - `/cases/`
   - `/cases/short-video-pipeline/`
   - `/tools/`
   - `/jiaorui/`
   - `/blog/`
   - `/about/`

