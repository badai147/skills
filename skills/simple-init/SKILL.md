---
name: simple-init
description: 快速总结项目的结构、技术栈与启动方式，并写入 AGENTS.md。进入新项目、接手陌生代码库、首次阅读仓库代码、需要快速了解项目全貌时使用。
license: MIT
---

## What I do

扫描项目关键文件，提炼项目是做什么的、核心技术栈、快速启动方式，写入 AGENTS.md，保持精炼（100-200 字）。

## 扫描优先级

按顺序查找，找到即可，不必全部读完：

1. README（README.md / README.zh-CN.md）— 项目定位与启动说明的最快来源
2. 包清单与配置 — package.json（重点看 scripts 的 dev/start/build）、pyproject.toml、go.mod、Cargo.toml、requirements.txt 等
3. 源码入口与部署文件 — src/ 主目录、main 入口、Dockerfile、docker-compose.yml
4. 文档目录 — docs/

## 输出格式

写入 AGENTS.md 时使用固定结构：

```
# 项目名
简介：一句话说明项目做什么、解决什么问题
技术栈：主要语言与框架
启动：可运行命令；找不到则写"见 README"
```

## 边界

- 项目已有 AGENTS.md：先读，在其基础上增补修正，不整体覆盖
- README 缺失：从配置与源码推断，不编造，不确定的信息写"未知"
- 宁缺毋滥：省略低价值细节，不写成流水账
