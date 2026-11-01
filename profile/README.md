<p align="center">
  <img src="https://hyloai.github.io/assets/logo.svg" width="72" alt="Hylo">
</p>

<h1 align="center">Hylo AI · 原觉智能</h1>

<p align="center">
  <b>Robot policies that improve behind a gate.</b><br>
  让机器人策略在统计门控下持续变好。
</p>

<p align="center">
  <a href="https://hyloai.github.io/">Website · 官网</a> ·
  <a href="https://hyloai.github.io/hylo-docs/">Docs · 文档</a> ·
  <a href="https://hyloai.github.io/hylo-docs/getting-started/quickstart/">Quickstart · 快速上手</a>
</p>

---

**Hylo** evaluates robot policies, learns from what they did, and promotes a change only when a paired statistical
test on episodes it never trained on says it is better. The approved version then runs on the robot through the same
episode loop it was measured with. One set of contracts from simulation (MuJoCo, LIBERO) to hardware (LeRobot robots),
for any policy (behaviour cloning, flow matching, SmolVLA, pi0).

**Hylo** 评测机器人策略，从它们的执行轨迹中学习；只有当一项改动在从未参与训练的回合上通过配对统计检验时，才会被采纳。
通过审批的版本随后在机器人上运行，用的正是度量它时的那套回合循环。从仿真（MuJoCo、LIBERO）到硬件（LeRobot 机器人），
适用于任何策略（行为克隆、流匹配、SmolVLA、pi0），用同一套契约。

### Repositories · 仓库

| Repository | What it holds | 内容 |
|---|---|---|
| [hylo-harness](https://github.com/HyloAI/hylo-harness) | the base: contracts, episode kernel, evaluation, agents, learning, campaigns, store, the `hylo` CLI | 底座：契约、回合内核、评测、智能体、学习、改进、存储、`hylo` 命令 |
| [hylo-bench](https://github.com/HyloAI/hylo-bench) | protocols, scorecards, leaderboards; MuJoCo and LIBERO | 跑分协议、记分卡、排行榜 |
| [hylo-serve](https://github.com/HyloAI/hylo-serve) | policy server, workcell, real-time runner, robot adapters | 策略服务器、workcell、机器人适配器 |
| [hylo-studio](https://github.com/HyloAI/hylo-studio) | run explorer, live sandbox, campaigns, workcell control | 运行浏览、实时沙箱、控制台 |
| [hylo-plugins](https://github.com/HyloAI/hylo-plugins) | example plugins | 示例插件 |
| [hylo-docs](https://github.com/HyloAI/hylo-docs) | documentation | 文档 |
| [hylo-deployments-template](https://github.com/HyloAI/hylo-deployments-template) | template for a lab's private workcell and safety configuration | 实验室私有配置模板 |

### Quick start · 快速上手

```bash
git clone https://github.com/HyloAI/hylo-harness.git harness
HYLO_GIT_BASE=https://github.com/HyloAI harness/dev/bootstrap.sh
uv run hylo run bench/examples/configs/mujoco_reach.yaml
```

Open source under the Apache License 2.0 · 以 Apache-2.0 许可开源 · [hyloai.io](https://hyloai.io)
