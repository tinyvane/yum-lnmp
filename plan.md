# yum-lnmp - LNMP 环境部署文档 - 项目规划

## 项目概述
Linux + Nginx + MySQL + PHP（LNMP）环境安装部署文档（Markdown 格式）。

---

## 2026-03-03 Claude 建议

### 建议

#### 文档更新
- LNMP 是较老的部署方案，部分配置可能已过时
- 建议更新 PHP 版本（PHP 8.2+）
- Nginx 配置更新（HTTP/2、TLS 1.3）
- MySQL 8.0 配置差异

#### 容器化替代
- 传统 LNMP → Docker Compose（更现代，更易管理）
```yaml
services:
  nginx:
  php:
  mysql:
```
- 参考 `20250904-projects-new` 的 Docker 配置

#### 整合方向
- 将 `yum-lnmp` + `deploymysql` + `aliyun_env_inst` 整合为**统一部署文档**
- 提供传统方式和 Docker 方式两种选择
