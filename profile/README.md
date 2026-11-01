<p align="center">
  <img src="https://hyloai.github.io/assets/logo.svg" width="72" alt="Hylo">
</p>

<h1 align="center">The Stack for Physical AI</h1>

<p align="center">
  <b>让具身智能运转起来</b>
</p>

<p align="center">
  <a href="https://hyloai.github.io/">Website · 官网</a> ·
  <a href="https://hyloai.github.io/hylo-docs/">Docs · 文档</a> ·
  <a href="https://hyloai.github.io/hylo-docs/getting-started/quickstart/">Quickstart · 快速上手</a>
</p>

---

From real-time running to cognition, evaluation and evolution, **Hylo** builds every layer of physical AI on one
execution kernel.

从实时运行到认知、评测、进化，**Hylo** 把具身智能的每一层建在同一个执行内核上。

### The Hylo stack · Hylo 技术栈

| Layer · 层 | | Repository · 仓库 |
|---|---|---|
| **Workbench · 工作台** | Run tasks, replay every episode and approve releases in one workspace.<br>在一个工作台里运行任务、回放每一次执行、批准发布。 | [hylo-studio](https://github.com/HyloAI/hylo-studio) |
| **Evolution · 进化** | Turn experience into stronger versions, each one tested before release.<br>把经验变成更强的版本，每一次都先检验再发布。 | [hylo-harness](https://github.com/HyloAI/hylo-harness) (learn, evolve) |
| **Evaluation · 评测** | Measure every policy against the same standard.<br>用同一把尺子衡量每一个策略。 | [hylo-bench](https://github.com/HyloAI/hylo-bench), [hylo-harness](https://github.com/HyloAI/hylo-harness) (eval) |
| **Cognition · 认知** | Use what the robot has seen and done to choose its next step.<br>让机器人用看到的和做过的，决定下一步。 | [hylo-harness](https://github.com/HyloAI/hylo-harness) (memory, agents, policies) |
| **Runtime · 运行** | Run policies on robots in real time, within the safety limits you set.<br>在你设定的安全边界内，让策略在机器人上实时运行。 | [hylo-serve](https://github.com/HyloAI/hylo-serve), [hylo-deployments-template](https://github.com/HyloAI/hylo-deployments-template) |
| **Kernel · 内核** | One execution kernel connects models, simulators and robots.<br>一个执行内核，接入模型、仿真器和机器人。 | [hylo-harness](https://github.com/HyloAI/hylo-harness) (core), [hylo-plugins](https://github.com/HyloAI/hylo-plugins) |

Documentation · 文档：[hylo-docs](https://github.com/HyloAI/hylo-docs)

### Quick start · 快速上手

```bash
git clone https://github.com/HyloAI/hylo-harness.git harness
HYLO_GIT_BASE=https://github.com/HyloAI harness/dev/bootstrap.sh
uv run hylo run bench/examples/configs/mujoco_reach.yaml
```

Open source under the Apache License 2.0 · 以 Apache-2.0 许可开源 · Hylo AI · 原觉智能
