set (CLICKHOUSE_BENCHMARK_SOURCES Benchmark.cpp)

set (CLICKHOUSE_BENCHMARK_LINK
    PRIVATE
        boost::program_options
        clickhouse_aggregate_functions
        clickhouse_common_config
        dbms
)

clickhouse_program_add(benchmark)

target_link_libraries (vxdfs-benchmark-lib PRIVATE vxdfs-client-lib)
