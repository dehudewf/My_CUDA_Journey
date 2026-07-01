# Roadmap

## Core Promise

100 天手撕 50 个 CUDA 算子，公开代码、手写笔记、实验环境、性能数据、失败记录和复盘结论。

## Phase 1: Element-wise Kernels

目标：建立 CUDA 程序的最小闭环，理解 thread、block、grid、global memory、边界判断和基础计时。

| Day | Kernel | Goal | Status |
|---:|---|---|---|
| 001 | Vector Add | 跑通第一个 CUDA kernel | Planned |
| 002 | Matrix Add | 理解二维索引和边界判断 | Planned |
| 003 | ReLU | 总结 element-wise 算子的共同模式 | Planned |
| 004 | Sigmoid | 观察数学函数和编译参数影响 | Planned |

## Phase 2: Reduction / Scan

目标：理解并行归约、同步、shared memory 和访存模式。

| Day | Kernel | Goal | Status |
|---:|---|---|---|
| 005 | Reduce Sum v1 | 写出 baseline | Planned |
| 006 | Reduce Sum v2 | 使用 shared memory | Planned |
| 007 | Weekly Review | 复盘第一周错误和概念 | Planned |

## Phase 3: GEMM Baseline

目标：从 naive GEMM 开始，逐步理解 tile、shared memory、memory coalescing 和性能瓶颈。

## Phase 4: Optimization

目标：逐步加入 shared memory tiling、vectorized load、bank conflict 分析、warp-level primitives。

## Phase 5: Attention-related Kernels

目标：把前面学到的基础算子和大模型推理场景关联起来。
