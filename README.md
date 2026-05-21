# dns-rules

一个自动化清洗、分类的 DNS 分流规则集，专为多出口 network 环境与 DNS 转发引擎（如 Mosdns）量身定制。

---

## 📌 数据源与更新机制

* **数据来源**：本项目的数据源基于公开的上游经典规则库 [Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)。
* **更新频率**：通过 GitHub Actions 工作流进行自动化数据清洗、扁平化提取与分拣，**每日定时自动更新**，确保规则的实时性。

---

## 📌 规则快捷链接 (jsDelivr CDN)

### 1. IP 规则
* [**中国本地网段 (`geoip_cn.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/ips/geoip_cn.txt)

### 2. 域名规则
* [**中国本地域名 (`geosite_cn.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/domains/geosite_cn.txt)
* [**Apple 中国直连域名 (`apple_cn.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/domains/apple_cn.txt)
* [**Google 中国直连域名 (`google_cn.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/domains/google_cn.txt)
* [**直连域名 (`direct_list.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/domains/direct_list.txt)
* [**代理域名 (`proxy_list.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/domains/proxy_list.txt)
* [**GFWList 域名 (`gfw_list.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/domains/gfw_list.txt)
* [**非中国域名 (`geolocation-no-cn.txt`)**](https://cdn.jsdelivr.net/gh/lo0pback-404/dns-rules@main/rules/domains/geolocation-no-cn.txt)

---

## 🚀 项目特性

* **纯净无状态**：规则仅包含纯文本域名或 IP 列表（一行一个）。
* **全球加速**：全线托管于 jsDelivr CDN，支持多分支网关设备（如 RouterOS、Linux）高速、稳定地拉取。
* **业务无感知**：配合策略路由或 DNS 转发分流，可有效优化跨国办公延迟并规避潜在的解析污染。

---

## ⚖️ 许可证

[MIT License](LICENSE)
