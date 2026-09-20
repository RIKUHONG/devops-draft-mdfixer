# AI 使用记录

## 记录 1：E2 交付物梳理

- 日期：2026-09-17
- 工具/模型：OpenAI Codex（具体模型由使用者按客户端显示补充）
- 任务：阅读 E2 PPT，整理 B 组 DRAFT、MDFixer 以及 A/B 共同交付内容。
- 提示摘要：确认第二次实验需要完成和上交的文件；使用 cJSON；本人负责 B 组 DRAFT 和 MDFixer。
- AI 建议：统一异步 Job、四类任务样例、artifact 引用、Backlog、ADR、AI 使用记录、个人贡献和校验脚本。
- 人工判断：采纳 PPT 明确要求；不把 HTTP API 实现当作 E2 必交内容；不虚构具体组号、姓名和配对组信息。
- 关联文件：本目录全部契约与文档。

## 记录 2：生成最小契约

- 日期：2026-09-17
- 工具/模型：OpenAI Codex（具体模型由使用者按客户端显示补充）
- 任务：生成最简单但覆盖全部要求的 E2 文件。
- 提示摘要：按确认的目录生成所有文件。
- AI 建议：使用 JSON Schema Draft 2020-12；状态使用 `QUEUED` 而不是 `PENDING`；cJSON 使用 CMake/CTest；固定完整提交 SHA。
- 人工采纳：采用 `QUEUED`、CMake/CTest、四十位 SHA 和标准库校验脚本。
- 人工修改：提交前应由本人填写真实身份、组号、Issue/PR，并与 A 组确认接口字段。
- 人工拒绝：拒绝伪造真实 Docker 镜像、实际构建日志、成员信息和联调结果；样例 URI 和摘要仅用于契约演示。
- 验证：运行 `python scripts/validate.py`，结果记录在 `validation-results.md`。

## 后续记录模板

每次 AI 辅助修改时追加：日期、工具/模型、任务、提示摘要、AI 建议、采纳/修改/拒绝理由、关联文件/提交和验证结果。
