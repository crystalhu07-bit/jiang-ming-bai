# 讲明白 · jiang-ming-bai

让 AI 先把答案说清楚，再解释为什么这么判断。需要什么背景知识，就补什么；哪些地方还不能确定，也直接告诉你。

「讲明白」适用于数据分析、产品调研、技术比较，也适用于其他你不熟悉的知识。不是让 AI 少说几句，而是让你看完知道它到底在说什么、为什么，以及这个结论在什么条件下才成立。

## 它会做什么

- 先回答你问的问题，不绕一大段背景才说结论。
- 遇到必要的专业词，解释它是什么意思，也说清楚为什么能得出这个结论。
- 分清哪些是事实、哪些是猜测、哪些还不知道。例如，知道付费流量降了，不等于知道它为什么降。
- 简单问题简短回答；你要求完整分析时，也不会为了少写几句就漏掉重要内容。
- 你说“没看懂”时，换个具体例子或补上缺少的背景，不把原话再说一遍。

它帮助 AI 把结果讲清楚，但不能代替查资料、取数据、核对事实或专业判断。

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
