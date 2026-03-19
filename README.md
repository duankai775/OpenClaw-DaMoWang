# 大魔王 OpenClaw - 一键安装 AI 技能平台

> 让每个人都能拥有强大的 AI 助手 | 36 个高级技能 | 单文件安装

---

## 🎉 欢迎使用大魔王 OpenClaw

**大魔王 OpenClaw** 是一个预配置的 OpenClaw 发行版，集成了 36 个高级 AI 技能，让你在 10 分钟内搭建完整的 AI 开发平台。

### ✨ 核心特性

- 🤖 **36 个技能开箱即用** - 从编程到设计，从搜索到监控
- 🧠 **知识库系统** - 114 篇文档索引， semantic 搜索
- 🔧 **零配置安装** - 不需要手动安装依赖、复制文件
- 🛡️ **企业级安全** - 自动修复 PowerShell 策略、权限管理
- 📊 **性能监控** - 内置 watchdog 监控系统健康
- 🎨 **品牌图标** - 大魔王专属安装界面

---

## 📦 下载安装

### 系统要求
- Windows 10/11 (64-bit)
- 管理员权限
- 互联网连接（首次需下载 Node.js 和 OpenClaw）

### 安装步骤

1. **下载** `大魔王OpenClaw安装程序.exe` (2.8 MB)
2. **右键** → 以管理员身份运行
3. **等待** 10 分钟（首次安装自动下载依赖）
4. **验证** 访问 http://localhost:18789

### 验证安装

安装完成后，打开命令提示符：

```batch
openclaw skills check
# 应看到: 24+ eligible skills

python %USERPROFILE%\.openclaw\workspace\tools\rebuild-index.py
# 应看到: OK: Indexed 114 docs, 537 unique terms

openclaw gateway status
# 应看到: Listening: 127.0.0.1:18789
```

---

## 🎯 包含的技能（36 个）

### 核心 AI 技能
- **ai-agent-orchestrator** - 多 Agent 协调
- **ai-code-assistant** - AI 编程助手
- **browser-control** - 浏览器自动化
- **desktop-automation** - 桌面自动化
- **workflow-orchestrator** - 工作流编排
- **knowledge-manager** - 知识库管理
- **model-router** - 多模型路由
- **perf-dashboard** - 性能监控
- **security-hardening** - 安全审计
- **self-improving-agent** - 自进化 Agent

### 深度学习 & ML
- **deep-learning-lab** - 深度学习实验
- **ml-algorithms** - 机器学习算法
- **custom-neural-modules** - 自定义神经网络
- **model-optimization** - 模型优化
- **model-quantization** - 模型量化
- **reinforcement-learning** - 强化学习
- **neural-architecture-search** - 神经架构搜索
- **neural-evolution** - 神经进化
- **graph-neural-networks** - 图神经网络
- **multimodal-learning** - 多模态学习

### Prompt & LLMOps
- **text-humanizer** - AI 文本人性化
- **prompt-engineering** - 提示工程
- **llm-deployment** - LLM 生产部署
- **langchain-framework** - LangChain 框架
- **llamaindex-rag** - LlamaIndex RAG
- **mind-neural-network** - 认知神经网络

### 工程 & 工具
- **data-engineering** - 数据工程
- **design-studio** - 设计工作室
- **ontology-manager** - 本体管理
- **ultimate-performance** - 极致性能
- **performance-tuning** - 性能调优
- **cross-platform-deployment** - 跨平台部署
- **evolver** - 自进化系统
- **evomap** - 技能进化地图
- **skill-creator** - 技能创建器

---

## 🔧 技术细节

### 自动安装内容
- OpenClaw v1.x (最新)
- Node.js 依赖自动检测
- PowerShell 执行策略自动设为 RemoteSigned
- 36 个技能复制到运行时目录
- Gateway 服务自动重启

### 配置说明
- **openclaw.json** - 已修复配置格式，支持 Ollama + OpenRouter
- **HEARTBEAT.md** - 自动化任务配置（每 6 小时知识更新等）
- **heartbeat-state.json** - 心跳状态跟踪

### 目录结构 (安装后)
```
%USERPROFILE%\.openclaw\workspace\
├── openclaw.json          # 主配置
├── HEARTBEAT.md           # 任务配置
├── skills\                # 36 个技能
├── knowledge/             # 知识库（空，需自行添加）
├── tools\                 # 工具脚本
│   └── rebuild-index.py   # 索引重建
└── memory\                # 记忆文件
```

---

## 🛠️ 常见问题

### Q: 安装失败/卡住？
**A:** 检查网络，确保能访问 npm 和 GitHub。可尝试手动安装 Node.js 后重试。

### Q: 技能无法使用？
**A:** 运行 `openclaw skills check` 查看缺失依赖。某些技能需要额外 Python 包。

### Q: 如何更新技能？
**A:** 重新运行 `大魔王OpenClaw安装程序.exe` 会覆盖，但保留 `knowledge/` 和 `memory/`。

### Q: 可以卸载吗？
**A:** 删除 `%USERPROFILE%\.openclaw\workspace\` 即可。干净彻底。

### Q: 支持 Mac/Linux？
**A:** 当前仅 Windows。其他平台可手动安装 OpenClaw，然后复制 `skills/` 文件夹。

---

## 📄 许可证

本软件基于 [OpenClaw](https://github.com/openclaw/openclaw) 构建，遵循 MIT 许可证。

© 2026 Great Demon King (大魔王)

---

## 🙏 致谢

- OpenClaw 团队 - 优秀的 AI 平台
- 所有开源贡献者
- 使用本软件的用户

---

**🚀 开始你的 AI 之旅！**  
如果遇到问题，欢迎提交 Issue 或联系作者。
