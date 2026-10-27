# 发布规则（强制）

本仓库任何 `git push` 之前，必须执行 `~/WorkBuddy/github-repos/RELEASE_RULES.md` 中的检查清单：

1. 确认本仓库档位（A 公开 / B 私有 / C 禁入）
2. 逐文件 `git status` 审查，禁止 `git add .`
3. 密钥扫描零命中（gitleaks / git secrets）
4. 敏感词扫描（手机号、邮箱、身份证、真实机构名）
5. 单文件 < 50MB，仓库总量 < 500MB

C 档内容（身份证、证书原件、仲裁材料、病历、信用报告、发票、密钥、BP 原文）**禁止进入本仓库**，用户口头授权也不例外。
