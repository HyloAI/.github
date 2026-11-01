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
| **Workbench** | Run tasks, replay every episode and approve releases in one workspace. | [hylo-studio](https://github.com/HyloAI/hylo-studio) |
| **Evolution** | Turn experience into stronger versions, each one tested before release. | [hylo-harness](https://github.com/HyloAI/hylo-harness) (learn, evolve) |
| **Evaluation** | Measure every policy against the same standard. | [hylo-bench](https://github.com/HyloAI/hylo-bench), [hylo-harness](https://github.com/HyloAI/hylo-harness) (eval) |
| **Cognition** | Use what the robot has seen and done to choose its next step. | [hylo-harness](https://github.com/HyloAI/hylo-harness) (memory, agents, policies) |
| **Runtime** | Run policies on robots in real time, within the safety limits you set. | [hylo-serve](https://github.com/HyloAI/hylo-serve), [hylo-deployments-template](https://github.com/HyloAI/hylo-deployments-template) |
| **Kernel** | One execution kernel connects models, simulators and robots. | [hylo-harness](https://github.com/HyloAI/hylo-harness) (core), [hylo-plugins](https://github.com/HyloAI/hylo-plugins) |

Documentation: [hylo-docs](https://github.com/HyloAI/hylo-docs)

### Quick start

```bash
git clone https://github.com/HyloAI/hylo-harness.git harness
HYLO_GIT_BASE=https://github.com/HyloAI harness/dev/bootstrap.sh
uv run hylo run bench/examples/configs/mujoco_reach.yaml
```

Open source under the Apache License 2.0 · Hylo AI
