# 医疗信息化专家包（顾问 + 端到端交付专家团）

把「医疗信息化项目怎么咨询、怎么交付」沉淀成可复用的 Agent 人设与流程。
自用为主，因此**不追求通用性，只追求在医院与卫健委的真实语境下能直接干活**。

## 内容

```
consultant/   医疗信息化咨询顾问（单体专家，顾安）
  agents/medical-it-consultant.md
  .codebuddy-plugin/plugin.json
  avatars/

delivery/     端到端交付专家团（主理人 + 4 名成员）
  agents/medical-it-delivery-team-lead.md    主理人（全康平，统筹交付）
  agents/medical-it-advisor.md               咨询顾问（沈博闻）
  agents/medical-it-architect.md             方案架构师（梁思远）
  agents/medical-it-data-expert.md           数据治理专家（柯源）
  agents/medical-it-delivery-manager.md      实施经理（施立）
  settings.json

dist/         可直接分发的安装包（无需克隆仓库）
  medical-it-consultant.zip
  medical-it-delivery.zip
```

## 能力覆盖

| 方向 | 主要内容 |
|---|---|
| 规划与系统集成 | HIS/EMR/LIS/PACS 选型、集成平台、医院信息化整体规划、网络架构 |
| 数据治理与互联互通 | 数据标准、互联互通测评、临床数据中心、专病库、主数据、指标口径 |
| AI + 医疗落地 | AI native 转型、医疗大模型、智能问诊、临床辅助决策落地路径 |
| 实施与运维 | 项目管理、等保合规、维保体系（传统维保 vs AI FDE）、故障响应 |

## 设计取向

- **项目语境优先**：人设里写的是真实工作流（售前调研 → 方案 → 招投标 → 实施 → 评级 → 回款），不是泛泛的「资深专家」
- **专家团有主理人**：多角色不是并列开会，而是有统筹、有交付责任边界
- **数据治理单列**：医疗项目里「数据」和「系统」是两套专业，混在一起必翻车（临床/科研数据中心、专病库、主数据、指标口径）

## 安装方式

**方式一：用发行包（推荐）**

下载 `dist/` 下对应的 zip，在 WorkBuddy 专家中心导入即可。

**方式二：直接拷目录**

把 `consultant/`、`delivery/` 复制进自定义专家目录，重命名后即可出现在专家列表：

```
~/.workbuddy/plugins/marketplaces/my-experts/plugins/
  medical-it-consultant/
  medical-it-delivery/
```

放好后需**完全退出 WorkBuddy（Cmd+Q）再重开**，专家列表在启动时加载，不会热更新。

## 更新记录

- 2026-11-03：补回 `delivery/settings.json`（团队主理人指向），重建发行包，重新校验注册
- 2026-10-27：仓库初始化

## 脱敏说明

本仓库内容已核对：**不含真实医院/卫健委/企业名称、不含客户数据、不含个人联系方式**。
头像为 AI 生成示意图。若你所在单位对方法论外传有要求，请在使用前自行评估。

## 可见性

当前为**私有仓库**。确认内容可公开后再转 public（Settings → Danger Zone → Change visibility）。

## License

内部使用（如需开源请先自行复核内容）
