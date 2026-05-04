# 一、DNS 配置

1. **回源地址（A 记录）**
   将 SaaS 回源指向源站 IP：
   **`saas -> 7.7.7.7`**

2. **优选 CNAME**
   配置 CDN 优选入口：
   **`cdn -> cf.090227.xyz`**

3. **待优选地址**
   定义需要进行链路优化的子域：
   **`123 -> 优选地址`**

4. **优选域名 CNAME**
   将业务域名接入优选链路：
  **`321 -> cdn.domain`**
> **⚠️回源地址和带优选地址的DNS记录要打开小黄云**

---

# 二、SaaS 配置

1. **配置回退源（Fallback Origin）**
   填写：
   **`saas.domain`**

2. **添加主机名（Custom Hostname）**
   自定义主机名：
   **`321.domain`**

3. **TLS 版本**
   选择 **TLS 1.2**（兼顾安全性与兼容性）

4. **验证方式**
   选择 **HTTP 验证**

5. **源服务器（Origin Server）**
   选择 **自定义（Custom）**，并填写：
   **`123.domain`**

---

# 三、效果对比

**优选前：**
![before](https://img.131714.xyz/file/blog/Saas/1HkXyE84.webp)

**优选后：**
![after](https://img.131714.xyz/file/blog/Saas/xo7LHi1Q.webp)

---
