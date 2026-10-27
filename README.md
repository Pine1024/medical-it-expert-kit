# 医疗信息化专家包（顾问 + 端到端交付专家团）

把"医疗信息化项目怎么咨询、怎么交付"沉淀成可复用的 Agent 人设与流程。
自用为主，因此**不追求通用性，只追求在医院与卫健委的真实语境下能直接干活**。

## 内容

```
consultant/   医疗信息化咨询顾问（单体专家）
  agents/medical-it-consultant.md
  .codebuddy-plugin/plugin.json
  avatars/

delivery/     端到端交付专家团（主理人 + 4 名成员）
  agents/medical-it-delivery-team-lead.md    主理人（统筹）
  agents/medical-it-advisor.md               咨询顾问
  agents/medical-it-architect.md             方案架构师
  agents/medical-it-data-expert.md           数据治理专家
  agents/medical-it-delivery-manager.md      实施经理
  settings.json
```

## 设计取向

- **项目语境优先**：人设里写的是真实工作流（售前调研 → 方案 → 招投标 → 实施 → 评级 → 回款），不是泛泛的"资深专家"
- **专家团有主理人**：多角色不是并列开会，而是有统筹、有交付责任边界
- **数据治理单列**：医疗项目里"数据"和"系统"是两套专业，混在一起必翻车（临床/科研数据中心、专病库、主数据、指标口径）

## 安装方式

放到 WorkBuddy 的自定义专家目录（`~/.workbuddy/plugins/marketplaces/my-experts/plugins/`）即可出现在专家列表。

## 脱敏说明

本仓库内容已核对：**不含真实医院/卫健委/企业名称、不含客户数据、不含个人联系方式**。
头像为 AI 生成示意图。若你所在单位对方法论外传有要求，请在使用前自行评估。

## 可见性

当前按 **B 档（私有）** 存放。确认内容可公开后再转 public。

## License

内部使用（如需开源请先自行复核内容）
