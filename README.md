# 灵犀后端 (Lingxi Backend)

FastAPI 多租户 SaaS 纯 API 服务（PostgreSQL + WebDAV + JWT 认证 + 独立计费）。

## 技术栈
- FastAPI + Uvicorn（单端口 8765）
- PostgreSQL 16（SQLAlchemy 2.0 async + asyncpg）
- WebDAV 文件存储（多租户隔离）
- JWT 认证 + bcrypt 密码哈希
- 多 Agent 编排（Orchestrator-Workers 模式）

## 部署
- Docker 镜像：`ghcr.io/mvpdark/lingxi-backend:latest`
- 环境变量配置见 `backend/.env.example`
- Unraid 模板见 `unraid/` 目录

## CI/CD
- 推送到 main 分支自动构建 Docker 镜像并推送到 GHCR
