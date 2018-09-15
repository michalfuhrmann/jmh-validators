`mvn clean install`
`java -jar target/benchmarks.jar -f 1 -i 10 -wi 10 -r 5`

Results:
Hibernate validators v5.2

| Benchmark                                | Mode | Cnt | Score   | Error | Units |
|------------------------------------------|------|-----|---------|-------|-------|
| ValidatorBenchmark._0_validate1Car       | avgt | 10  | ≈ 10⁻⁵  |       | s/op  |
| ValidatorBenchmark._1_validate10Car      | avgt | 10  | ≈ 10⁻⁴  |       | s/op  |
| ValidatorBenchmark._2_validate100Car     | avgt | 10  | 0.003 ± | 0.001 | s/op  |
| ValidatorBenchmark._3_validate1000Car    | avgt | 10  | 0.021 ± | 0.001 | s/op  |
| ValidatorBenchmark._4_validate10_000Car  | avgt | 10  | 0.301 ± | 0.004 | s/op  |
| ValidatorBenchmark._5_validate100_000Car | avgt | 10  | 2.986 ± | 0.107 | s/op  |

Hibernate validators v6.0

| Benchmark                                | Mode | Cnt | Score   | Error | Units |
|------------------------------------------|------|-----|---------|-------|-------|
| ValidatorBenchmark._0_validate1Car       | avgt | 10  | ≈ 10⁻⁶  | s/op  | s/op  |
| ValidatorBenchmark._1_validate10Car      | avgt | 10  | ≈ 10⁻⁵  | s/op  | s/op  |
| ValidatorBenchmark._2_validate100Car     | avgt | 10  | ≈ 10⁻⁴  | s/op  | s/op  |
| ValidatorBenchmark._3_validate1000Car    | avgt | 10  | 0.002 ± | 0.001 | s/op  |
| ValidatorBenchmark._4_validate10_000Car  | avgt | 10  | 0.016 ± | 0.001 | s/op  |
| ValidatorBenchmark._5_validate100_000Car | avgt | 10  | 0.165 ± | 0.003 | s/op  |
