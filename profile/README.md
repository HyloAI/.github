<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg">
    <img src="assets/banner-light.svg" width="100%" alt="Hylo: the stack for physical AI. Every layer on one execution kernel">
  </picture>
</p>

<p align="center">
  <a href="https://hyloai.github.io/"><b>Website</b></a> ·
  <a href="https://hyloai.github.io/hylo-docs/"><b>Docs</b></a> ·
  <a href="https://hyloai.github.io/hylo-docs/getting-started/quickstart/"><b>Quickstart</b></a>
</p>

From real-time running to cognition, evaluation and evolution, **Hylo** builds every layer of physical AI on one
execution kernel.

Hylo helps teams develop, validate, deploy and accumulate robot skills: reusable task capabilities with stated
applicability, executable implementations and measured evidence. Robot tools, programs and existing policies
share execution, evaluation and versioning infrastructure.

[Robot skills and their lifecycle](https://hyloai.github.io/hylo-docs/user-guide/skills/) ·
[Develop a robot skill](https://hyloai.github.io/hylo-docs/user-guide/developing-strategies/) ·
[Run an existing policy](https://hyloai.github.io/hylo-docs/getting-started/quickstart/) ·
[Skill research, validation and reuse](https://hyloai.github.io/hylo-docs/user-guide/research-and-skills/) ·
[Tool-calling agents](https://hyloai.github.io/hylo-docs/user-guide/tool-agents/) ·
[Robot worlds](https://hyloai.github.io/hylo-docs/user-guide/worlds/)

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/loop-dark.svg">
    <img src="assets/loop-light.svg" width="100%" alt="The Hylo loop: run, measure, improve through a gate, deploy; episodes on the robot come back as runs">
  </picture>
</p>

### The Hylo stack

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="assets/stack-dark.svg">
    <img src="assets/stack-light.svg" width="100%" alt="The six layers of the Hylo stack and the repositories that implement them">
  </picture>
</p>

| Layer | | Repository |
|---|---|---|
| **Workbench** | Inspect skill development, validation evidence and deployed execution. | [hylo-studio](https://github.com/HyloAI/hylo-studio) |
| **Evolution** | Improve skill implementations with learning, experiments and versioned promotion. | [hylo-harness](https://github.com/HyloAI/hylo-harness) (learn, evolve) |
| **Evaluation** | Validate skill implementations under fixed protocols and stated conditions. | [hylo-bench](https://github.com/HyloAI/hylo-bench), [hylo-harness](https://github.com/HyloAI/hylo-harness) (eval) |
| **Cognition** | Implement robot skills with tools, programs, policies and memory. | [hylo-harness](https://github.com/HyloAI/hylo-harness) (manip, agents, policies, memory) |
| **Runtime** | Run skill implementations on robots within configured safety limits. | [hylo-serve](https://github.com/HyloAI/hylo-serve), [hylo-deployments-template](https://github.com/HyloAI/hylo-deployments-template) |
| **Kernel** | One execution kernel connects models, simulators and robots. | [hylo-harness](https://github.com/HyloAI/hylo-harness) (core), [hylo-plugins](https://github.com/HyloAI/hylo-plugins) |

Documentation: [hylo-docs](https://github.com/HyloAI/hylo-docs)

### Quick start

```bash
git clone https://github.com/HyloAI/hylo-harness.git harness
HYLO_GIT_BASE=https://github.com/HyloAI harness/dev/bootstrap.sh
uv run hylo run bench/examples/configs/mujoco_reach.yaml
```

Open source under the Apache License 2.0 · Hylo AI
