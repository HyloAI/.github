<p align="center">
  <img src="https://hyloai.github.io/assets/logo.svg" width="72" alt="Hylo">
</p>

<h1 align="center">Hylo AI · 原觉智能</h1>

<p align="center">
  <b>Robots that keep getting better as they work.</b><br>
  让机器人在使用中持续变好。
</p>

<p align="center">
  <a href="https://hyloai.github.io/">Website · 官网</a> ·
  <a href="https://hyloai.github.io/hylo-docs/">Docs · 文档</a> ·
  <a href="https://hyloai.github.io/hylo-docs/getting-started/quickstart/">Quickstart · 快速上手</a>
</p>

---

**Hylo** turns a robot's own work into its next improvement. Every episode is recorded in full. Changes are learned
from those records, checked against the current version on episodes they have never seen, and only then sent to the
robot. The benchmark and the robot run through the same episode loop, with the same timing.

**Hylo** 把机器人自己的工作，变成它下一次改进的依据。每个回合都被完整记录下来；改动从这些记录中学出来，先在它从没见过的回合上
和当前版本对比，通过了才交给机器人。基准测试和真机跑的是同一套回合循环，时序也一样。

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
