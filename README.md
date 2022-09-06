# PyO3-chrono PRs benchmarks

This repo is used to benchmark two possible implementations of the PyO3-chrono integration.

# Usage

Clone this repository: 

```bash
git clone <>
```

Init the submodules:
```bash
git submodule update --init --recursive
```

Benchmark the two different implementations:

```bash
git co pyo3-pickfire
cargo bench --bench bench_chrono_integration
git co pyo3-psykopear
cargo bench --bench bench_chrono_integration
```
