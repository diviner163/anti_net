# CF Worker 智能订阅系统

专为全球网络环境优化的高性能节点管理系统。

## 特性

- 🛡️ 网络优化机制
  - 智能DNS解析
  - 连接稳定性增强
  - 多端口支持
  - 协议优化

- 🔄 连接质量提升
  - 智能DNS缓存
  - 路由优化
  - 故障转移
  - 延迟优化

- 🚀 性能保障
  - 节点状态监控
  - 负载均衡
  - 智能缓存
  - 并发处理

## 部署步骤

### 1. 前置需求
- Cloudflare 账号
- 自定义域名（推荐）
- GitHub 账号

### 2. 配置文件准备
1. Fork 本仓库
2. 修改配置文件：
   - `config/config.json`: 基础配置
   - `config/china.json`: 中国网络优化配置
   - `config/security.json`: 安全配置

### 3. 节点配置
1. 编辑 `endpoints/tls.txt` 和 `endpoints/notls.txt`
2. 添加您的节点信息，格式：
   ```
   域名#备注（延迟）#备用域名
   ```

### 4. Workers 部署
1. 登录 Cloudflare Dashboard
2. 创建新的 Worker
3. 复制 `worker.js` 内容
4. 部署 Worker

### 5. 域名绑定（推荐）
1. 在 Workers 设置中添加自定义域名
2. 配置 DNS 记录指向 Workers

## 使用说明

### 基础访问
- `/auto` - 自动选择最优节点
- `/hk` - 香港节点
- `/sg` - 新加坡节点
- `/jp` - 日本节点

### 高级参数
- `?timeout=3000` - 设置超时时间
- `?area=hk,jp` - 指定地区
- `?exclude=sg` - 排除地区

## 安全配置

### 速率限制
