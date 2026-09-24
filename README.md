# Multi-Agent DDPG in PettingZoo

A PyTorch implementation of MADDPG and a MADDPG approximation variant for cooperative and competitive Multi-Agent Particle Environments.

## Problem and method

Multiple agents act simultaneously in a shared environment. Centralized critics use joint information during learning, while actors select each agent's actions. The upstream code compares variants on cooperative navigation, physical deception, and predator-prey tasks.

## Repository map

| Path | Purpose |
| --- | --- |
| `maddpg/` | Agent and model implementation |
| `train.py`, `train_parallel_env.py` | Training entry points |
| `run.py` | Playback and evaluation entry point |
| `plot.py`, `outputs/` | Existing comparison plots and GIFs |
| `environment.yml` | Dependency specification |

## Existing upstream outputs

![Upstream cooperative-navigation rollout](outputs/gifs/simple_spread_v3/MADDPG_all_episodes.gif)

![Upstream algorithm comparison](outputs/plots/compare/simple_spread_v3_algorithm_comparison.png)

These animations and plots are supplied by the original project; no new episodes or plots were generated here. The [upstream README](UPSTREAM_README.md) includes commands for the three environments and analysis of MADDPG versus MADDPG-Approx.

## Source and license

Based on and adapted from [legalaspro/maddpg-zoo-torch](https://github.com/legalaspro/maddpg-zoo-torch). The original documentation, references, and [MIT license](LICENSE) are retained.