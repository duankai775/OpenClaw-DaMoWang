# 大魔王 OpenClaw Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-03-19

### Added
- ✅ 首次公开发布
- ✅ 36 个核心 AI 技能预配置
- ✅ 一键安装程序（单文件 EXE，2.8 MB）
- ✅ 自动修复 OpenClaw 配置问题
- ✅ PowerShell 执行策略自动优化
- ✅ 内置知识库索引工具（114 篇文档）
- ✅ 性能监控守护进程（watchdog）
- ✅ 系统恢复脚本（restore-system.bat）
- ✅ 大魔王品牌图标（👑）
- ✅ 完整中文文档

### Technical Details
- **Base**: OpenClaw latest
- **Skills**: 36 (including knowledge-manager, model-router, perf-dashboard, security-hardening)
- **Config**: Fixed openclaw.json (model array format, plugin name)
- **Installation**: Automated, 10 minutes first-time
- **Platform**: Windows 10/11 (64-bit)

### Known Issues
- Ollama 模型需替换为支持 tools 的版本（如 llama3:8b）
- OPENROUTER_API_KEY 未设置（不影响基本功能）
- knowledge/ 文件夹初始为空（用户需自行添加内容）

---

## 📦 文件清单

```
大魔王OpenClaw安装程序.exe    (2.8 MB) - 主安装包
README.md                    (3.3 KB) - 使用说明
LICENSE                     (1.1 KB) - MIT 许可证
CHANGELOG.md                (2.4 KB) - 版本历史
```

---

## 🔮 未来计划

- [ ] 添加 Mac/Linux 支持
- [ ] 集成更多预训练模型
- [ ] 提供 Docker 镜像
- [ ] 创建 Web UI 管理界面
- [ ] 技能市场集成
- [ ] 多语言支持（英文、日文等）

---

**Built with ❤️ by Great Demon King**
