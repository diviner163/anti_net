# CF Worker 智能订阅系统

一个基于 Cloudflare Workers 的高性能节点管理系统。

## 功能特点

- ⚡️ 智能节点优选
- 🔄 自动故障转移
- 📊 实时性能监控
- 🛡️ 内置安全防护
- 🌐 智能路由优化
- 🚀 自动负载均衡

## 快速部署

### 1. 准备工作
- Cloudflare 账号
- Workers 服务已启用
- GitHub 账号（用于存储配置）

### 2. 部署步骤

1. **Fork 本仓库**
   - 访问 GitHub 仓库
   - 点击右上角 Fork 按钮

2. **创建 Worker**
   - 登录 Cloudflare Dashboard
   - 进入 Workers & Pages
   - 点击 "Create Application"
   - 选择 "Create Worker"

3. **部署配置**
   - 复制 `worker.js` 内容到 Worker
   - 点击 "Save and Deploy"

4. **自定义域名**（可选）
   - Workers → 选择你的 Worker
   - 点击 "Triggers"
   - 添加自定义域名

### 3. 使用方法

访问以下路径获取节点：
- `/auto` - 自动选择最优节点
- `/r1` - 区域1节点
- `/r2` - 区域2节点
- `/r3` - 区域3节点

## 注意事项

1. 确保 Worker 配置正确
2. 定期更新节点信息
3. 监控系统性能
4. 及时处理错误日志

## License

MIT License

## 支持

如有问题，请提交 Issue 或 Pull Request
