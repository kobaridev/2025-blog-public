## 一、前期准备

1. **Tailscale**：[官网下载](https://tailscale.com/download)

2. **Windows 专业版**：远程桌面（RDP）功能仅专业版及以上支持

   - 可参考：[家庭版升专业版教程](https://blog.131714.xyz/blog/mas)

3. **控制端**

   - 移动端：下载 Microsoft Remote Desktop（应用商店搜索）

   - Windows：远程桌面连接（自带）

> ⚠️ **控制端同样需要安装 Tailscale（重要）**

------

## 二、Tailscale 配置

1. 官网下载，安装一路点击 next

2. 登录微软账号（或 Google / GitHub 均可）

3. 开启开机自启动（保证远程设备随时在线）

4. **所有设备统一要求（关键补充）**

   - 控制端 + 被控端 **都必须安装 Tailscale**
   - 并且 **登录同一个账号**
   - 才能处于同一个虚拟局域网（Tailnet）

5. **获取设备 IP（重要）**

   - 在 Tailscale 客户端中查看

   - 格式一般为：

     ```
     100.x.x.x
     ```

------

## 三、连接方式

### Windows 控制端

1. 打开远程桌面连接（mstsc）

2. 输入 Tailscale IP：

   ```
   100.x.x.x
   ```

3. 输入账号密码连接

### 移动端

1. **先安装并登录 `Tailscale`（与电脑相同账号）**
2. 打开 `Windows App`
3. 添加 PC
   - PC Name：Tailscale IP
   - User：Windows 账号
4. 点击连接

------