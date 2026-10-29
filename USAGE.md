# OpenCode 机器人使用说明

这个仓库接入了 OpenCode 的 GitHub 集成：在 issue 或 PR 里评论 `/oc ...`，机器人会在 GitHub Actions 里执行任务并回复。

## 用法

| 场景 | 评论内容 |
| --- | --- |
| 解释问题 | `/oc 解释一下这个 issue` |
| 修 bug | `/oc 修复这个问题`（会开分支并提 PR） |
| 改代码 | 在 PR 里评论 `/oc 把这里的错误处理补上` |

`/opencode` 与 `/oc` 等价。

## 配置

| 项目 | 值 |
| --- | --- |
| workflow | `.github/workflows/opencode.yml` |
| 模型 | `opencode/deepseek-v4.1-flash-free`（免费） |
| 密钥 | 不需要 |

换模型只需修改 workflow 里的 `model:` 一行。免费模型列表见 <https://opencode.ai/docs/zen/>。
