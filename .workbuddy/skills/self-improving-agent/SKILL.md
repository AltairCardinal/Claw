# self-improving-agent

一个帮助AI编码助手实现自我改进的技能。

## 功能

- 记录错误、学习经验、功能请求
- 支持知识提升到项目内存文件
- 重复模式检测
- 多代理兼容

## 使用

当遇到以下情况时，按格式记录到对应文件：

### 错误记录 (ERRORS.md)
```markdown
- [2026-03-22 21:00] [high] [open] 命令执行失败
  - 命令: `npm install`
  - 错误: EACCES permission denied
  - 解决: 使用 `sudo` 或修复 npm 权限
```

### 学习记录 (LEARNINGS.md)
```markdown
- [2026-03-22 21:00] [correction] [p1] [open] 纠正行为
  - 用户反馈: 应该使用绝对路径而非相对路径
  - 建议: 优先使用绝对路径
```

### 功能请求 (FEATURE_REQUESTS.md)
```markdown
- [2026-03-22 21:00] [p2] [open] 添加自动化测试
  - 描述: 为项目添加 CI/CD 测试流程
```

## 文件位置

- `.learnings/LEARNINGS.md` - 学习记录
- `.learnings/ERRORS.md` - 错误记录
- `.learnings/FEATURE_REQUESTS.md` - 功能请求

## 版本

v3.0.5 (简化版)
