# Contributing

This repo is primarily a learning-in-public archive. Contributions should keep the project reproducible and honest.

## Add a New Kernel

Create this structure:

```text
kernels/dayXXX-kernel-name/
├── README.md
├── kernel.cu
├── benchmark.py
└── result.csv
```

Then update:

1. `README.md` kernel registry.
2. `PROGRESS.md`.
3. `benchmarks/summary.csv` if benchmark data exists.
4. `notes/dayXXX-kernel-name.md`.

## Required Evidence

Every benchmark must include:

- GPU model.
- CUDA version.
- Driver version.
- Compiler and flags.
- Input shape.
- DType.
- Timing method.
- Baseline.

## Status Rules

Do not mark a kernel as:

- `Code` until source code exists.
- `Verified` until correctness test passes.
- `Benchmarked` until raw benchmark data is committed.
- `Explained` until the note explains mechanism, bug, and boundary.

## Writing Rules

1. Keep build commands runnable.
2. Keep benchmark claims scoped to the recorded environment.
3. Record failed runs if they block progress.
4. Prefer small, verifiable steps over large tutorial-style rewrites.
