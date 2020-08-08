![CI](https://github.com/LesnyRumcajs/grpc_bench/workflows/CI/badge.svg)

One repo to finally have a clear, objective gRPC benchmark with code for everyone to verify and improve.

Contributions are most welcome!

# Prerequisites
Linux or MacOS with Docker. Keep in mind that the results on MacOS may not be that reliable, Docker for Mac runs on a VM.

# Running benchmark
To build the benchmarks images use: `./build.sh [BENCH1] [BENCH2] ...` . You need them to run the benchmarks.

To run the benchmarks use: `./bench.sh [BENCH1] [BENCH2] ...` . They will be run sequentially.

To clean-up the benchmark images use: `./clean.sh [BENCH1] [BENCH2] ...`

## Configuring the benchmark
Benchmark duration is governed by environmental variable `GRPC_BENCHMARK_DURATION`. Defaults to `30s`.

The maximum number of cpus used by server is governed by the environmental variable `GRPC_SERVER_CPUS`. Defaults to `1`.

# Results
You can find our sample results in the [Wiki](https://github.com/LesnyRumcajs/grpc_bench/wiki). Be sure to run the benchmarks yourself if you have sufficient hardware, especially for multi-core scenarios.
