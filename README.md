# PyO3-chrono PRs benchmarks

This repo is used to benchmark two possible implementations of the PyO3-chrono integration.

# Usage

Clone this repository: 

```bash
git clone git@github.com:Psykopear/pyo3-chrono-benches.git
```

Init the submodules:
```bash
git submodule update --init --recursive
```

Benchmark the two different implementations:

```bash
git checkout pickfire
git submodule update
cargo bench --manifest-path pyo3/Cargo.toml --bench bench_chrono_integration
git checkout psykopear
git submodule update
cargo bench --manifest-path pyo3/Cargo.toml --bench bench_chrono_integration
```
