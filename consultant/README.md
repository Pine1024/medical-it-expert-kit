# 医信顾问（MedIT Advisor）

医疗行业信息化咨询专家：从医院信息化规划、系统集成、数据治理与互联互通，到 AI+医疗落地与实施运维，提供全链路咨询建议。

## 类型

Agent 型（单个 AI 专家）

## 功能

- 医院信息化整体规划与 HIS/EMR/LIS/PACS 核心系统选型、集成与升级路径
- 数据治理、互联互通标准化成熟度测评与电子病历分级评价准备
- AI+医疗落地评估：医疗大模型、智能问诊、临床辅助决策的可行性与部署方案
- 选型与架构评估：模型能力、开发方式（自研/合作/采购）、供应商性价比、私有云/公有云/混合云架构
- 实施运维与维保咨询：项目管理、传统维保与 AI FDE 交付模式对比、故障响应体系

## 使用示例

- 我们医院想升级现有HIS系统，现有系统老旧且数据分散，请帮我做一份信息化规划建议。
- 医疗数据互联互通标准化成熟度测评应该怎么准备？
- 医院计划落地AI辅助诊断，应该选私有云还是公有云部署？

## 头像

头像已自动生成在 `avatars/` 目录下。如需替换为自定义头像，要求：
- 格式：PNG（推荐）或 JPG
- 尺寸：512×512 px
- 大小：单张不超过 500KB

## 安装

将专家包目录放到专家目录下：

```
/Users/pine/.workbuddy/plugins/marketplaces/my-experts/plugins/medical-it-consultant/
```

然后运行注册命令使其可见：

```bash
python3 scripts/register_expert.py <expert-dir>
```

## 打包分享

```bash
python3 scripts/package_expert.py <expert-dir>
```
