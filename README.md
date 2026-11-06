# 讲明白 · jiang-ming-bai

让 AI 的调研、分析和专业解释更容易理解：先回答问题，再说明依据和必要背景，保留关键条件与不确定性。

不是一味缩短答案，也不是把专业内容变成口号。适用于数据分析、产品调研、技术比较和其他知识话题。

## 它会做什么

- 先给出有依据的结论，不用大段主题介绍代替答案。
- 解释必要术语，补上证据与结论之间的推理。
- 区分事实、推断与未知，避免把流量变化直接说成已查明的原因。
- 根据问题决定篇幅：简单问题简答，完整调研不遗漏必要维度。
- 用户反馈“没看懂”时，换具体例子或补必要背景，而非重复原话。

它负责回答的组织和解释，不替代研究、取数、事实核验或专业判断。

## 安装

下载本仓库 ZIP 并解压，将包含 `SKILL.md` 和 `references/` 的文件夹重命名为 `jiang-ming-bai`，放入对应用户级目录：

| 客户端 | 目录 |
|---|---|
| Codex | `~/.codex/skills/jiang-ming-bai/` |
| Claude Code | `~/.claude/skills/jiang-ming-bai/` |

`~` 表示用户主目录。Windows 可在用户主目录下找到或新建对应的 `.codex/skills` 或 `.claude/skills` 目录。若已有同名技能，先备份再更新，不要直接覆盖个人改动。

也可以在 macOS / Linux 终端中选择一条命令安装（需要 Git，目标目录必须不存在）：

```bash
# Codex
git clone https://github.com/crystalhu07-bit/jiang-ming-bai.git ~/.codex/skills/jiang-ming-bai
```

```bash
# Claude Code
git clone https://github.com/crystalhu07-bit/jiang-ming-bai.git ~/.claude/skills/jiang-ming-bai
```

安装后重启客户端并新建对话，以便重新发现技能。

## 使用

可以明确要求：

> 使用讲明白（jiang-ming-bai）解释：RAG 和微调有什么区别？公司制度每周更新，该怎么选？

技能描述也支持客户端在相关分析和解释任务中自动选择；是否实际触发取决于客户端和模型，不能保证每次都会自动调用。

## 文件

- [SKILL.md](SKILL.md)：核心规则。
- [回答示例](references/examples.md)：数据分析、专业机制、证据不足和短答示范，均为教学假设。
- [质量测试](references/quality-tests.md)：评估场景和验收标准。

## 验证与反馈

已通过结构校验，并在 Codex 中进行过一轮 7 个场景的有／无技能对照，修正并重测了数据解释中的一处问题。这不是普遍有效的证明；Claude Code 下的实际表现、自动触发稳定性及长期用户体验仍需验证。

反馈时建议提供脱敏后的问题和回答，并指出具体障碍：结论不明确、术语难懂、推理跳步、篇幅冗长或过度简化。请勿提交密码、客户数据或公司保密资料。
