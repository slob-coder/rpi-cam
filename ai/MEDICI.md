# 项目地图 — AI视频生成平台

## 目录结构
```
ai/
├── requirements-spec.md    # 需求规格文档
├── MEDICI.md               # 项目地图（本文件）
├── architecture.md         # 架构设计（待 architect 产出）
├── src/                    # 源代码（待 coder 产出）
│   ├── frontend/           # Next.js + React 前端
│   ├── backend/            # FastAPI 后端
│   └── ...
└── tests/                  # 测试代码（待 tester 产出）
```

## 文档索引
| 文档 | 路径 | 说明 |
|------|------|------|
| 需求规格文档 | ai/requirements-spec.md | 功能级需求定义，含 15 个功能点 |
| 架构设计 | ai/architecture.md | 待 architect 产出 |
| 项目地图 | ai/MEDICI.md | 本文件 |

## 功能清单
| ID | 功能名 | 优先级 | 状态 |
|----|--------|--------|------|
| F01 | AI脚本生成 | P0 | requirements_defined |
| F02 | 脚本编辑与版本管理 | P0 | requirements_defined |
| F03 | 智能分镜拆分 | P0 | requirements_defined |
| F04 | 分镜手动调整 | P1 | requirements_defined |
| F05 | AI画面描述生成 | P1 | requirements_defined |
| F06 | 参考图片上传 | P2 | requirements_defined |
| F07 | 音频转字幕 | P0 | requirements_defined |
| F08 | 字幕多语言翻译 | P1 | requirements_defined |
| F09 | 字幕样式编辑 | P1 | requirements_defined |
| F10 | 字幕格式导出 | P1 | requirements_defined |
| F11 | 视频素材组合 | P0 | requirements_defined |
| F12 | 转场效果与背景音乐 | P1 | requirements_defined |
| F13 | 多分辨率输出 | P1 | requirements_defined |
| F14 | 视频实时预览 | P0 | requirements_defined |
| F15 | 用户注册登录 | P0 | requirements_defined |
| F16 | 项目管理 | P0 | requirements_defined |
| F17 | 多人协作 | P2 | requirements_defined |

## 架构概览
- **前端**: Next.js + React（SSR + SPA 混合模式）
- **后端**: FastAPI + PostgreSQL（RESTful API + WebSocket 实时通信）
- **存储**: S3 兼容对象存储（视频/图片/音频等媒体资源）
- **AI 服务**: OpenAI（脚本生成）、Runway（视频生成）、ElevenLabs（语音合成）、Whisper（语音转文字）
- 详细架构设计待 architect 产出 → architecture.md

## 技术栈约束
| 层级 | 技术选型 |
|------|----------|
| 前端框架 | Next.js + React |
| 后端框架 | FastAPI |
| 数据库 | PostgreSQL |
| 对象存储 | S3 兼容 |
| AI-脚本 | OpenAI GPT |
| AI-视频 | Runway |
| AI-语音 | ElevenLabs |
| AI-字幕 | Whisper |
