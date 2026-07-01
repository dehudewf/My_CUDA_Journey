# Environment

Record every important version before publishing a benchmark.

```text
OS:
GPU:
Driver:
CUDA:
nvcc:
Python:
PyTorch:
Compiler:
```

## Benchmark Rules

1. Always record GPU model.
2. Always record input shape and dtype.
3. Always record timing method.
4. Compare only under the same hardware, input size, dtype, and measurement method.
5. Keep raw results in `benchmarks/`.
