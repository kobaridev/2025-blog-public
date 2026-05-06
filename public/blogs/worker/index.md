# 一、配置 Worker 路由 (Route)
1. 进入 Cloudflare Worker 控制台，选择目标 Worker 并在 **设置 (Settings)** 选项卡中找到 **Domains & Routes**。
2. 点击 添加，选择**路由**。
3. 按照以下参数进行设置：
   *  **Zone (区域)：** `xzzya.de5.net`
   *  **Route (路由)：** `yx.xzzya.de5.net/*`
4. 点击 **保存/更新路由 (Update route)**。

# 二、配置 DNS 解析 (CNAME)
1. 切换至 `xzzya.de5.net` 域名的 **DNS** 管理界面。
2. 添加一条 **CNAME** 记录：
   *  **名称 (Name)：** `yx`
   *  **目标 (Target)：** `cf.090227.xyz`
   *  **代理状态：** 建议关闭（橙色小云朵）。

---