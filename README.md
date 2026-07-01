# My CUDA Journey

> 100 天手撕 50 个 CUDA 算子，记录代码、手写笔记、性能数据、失败过程和复盘结论。

## Why

CUDA 对新手最大的难点不是语法，而是看不见 GPU 在怎么执行。

这个仓库尝试用最小可运行代码、手写图解和 benchmark 数据，把 CUDA 学习过程拆成一个个可复现的小实验。

我不会把这里包装成“教程大全”，而是公开记录自己的学习路径：每天实现一个小 kernel，说明它解决什么问题、怎么运行、哪里容易错，以及下一步如何优化。

## Progress

| 阶段 | 主题 | 状态 |
|---|---|---|
| Phase 1 | Element-wise kernels | 进行中 |
| Phase 2 | Reduction / Scan | 未开始 |
| Phase 3 | GEMM baseline | 未开始 |
| Phase 4 | Shared memory optimization | 未开始 |
| Phase 5 | Attention-related kernels | 未开始 |

## Daily Log

| Day | Kernel | Code | Note | Benchmark | Bugs |
|---:|---|---|---|---|---|
| 001 | Vector Add | `kernels/day001-vector-add/` | `notes/day001-vector-add.md` | `benchmarks/day001-vector-add.csv` | `bugs/day001-build-error.md` |
| 002 | Matrix Add | `kernels/day002-matrix-add/` | `notes/day002-matrix-add.md` | - | - |

## Repository Structure

```text
kernels/      每天的 CUDA kernel 源码与运行脚本
notes/        每天的学习笔记和每周复盘
benchmarks/   原始性能数据
bugs/         报错、排查和修复记录
images/       手写笔记、图解和结果截图
platform/     知乎、CSDN、小红书分发稿
templates/    内容模板
```

## Environment

See `ENVIRONMENT.md`.

```text
OS:
GPU:
Driver:
CUDA:
nvcc:
Python:
PyTorch:
```

## Platform Notes

- GitHub: source of truth.
- Zhihu: principles, tradeoffs, and learning reflections.
- CSDN: build steps, reproducible commands, and bugs.
- Xiaohongshu: visual notes and weekly progress.

## Rules

1. No benchmark without hardware, input size, and measurement method.
2. No copied tutorial without personal experiment.
3. Every bug worth recording if it blocks reproduction.
4. Keep code runnable before making the note pretty.
