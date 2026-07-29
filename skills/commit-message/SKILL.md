---
name: commit-message
description: 根据 git diff 生成符合项目历史风格的 commit message
license: MIT
---

1. 执行 `git diff --staged` 或 `git diff` 获取变更
2. 分析近期 10 条 commit 日志，识别格式惯例
3. 生成一条 message，遵循项目历史风格，不强制限制长度
