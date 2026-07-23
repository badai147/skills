---
name: commit-message
description: 根据 git diff 生成符合项目历史风格的 commit message
license: MIT
---

## What I do

1. 执行 `git diff --staged` 或 `git diff` 获取变更
2. 分析近期 10 条 commit 日志，识别格式惯例（如 type(scope): subject）
3. 生成一条精炼（50字符内）且风格一致的 message，subject 为中文
