# 202individualassignment

## Build
Requires Java 17+ and Maven.
```
mvn clean package
```

## Run
```
java -jar target/analyzer.jar --file samples/events.txt --outdir results/
```
- `--file`: input file (required)
- `--outdir`: output directory (optional, default: current directory)

## Percentile method
Percentiles use the nearest-rank method. For a sorted list of N values, the p-th
percentile is the value at index `ceil(p/100 * N) - 1` (0-indexed).
