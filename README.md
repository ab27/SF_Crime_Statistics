1. How did changing values on the SparkSession property parameters affect the throughput and latency of the data?

* It gave differnt values for inputRowsPerSecond and processedRowsPerSecond in the Progress Report: 

2. What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?

* spark.default.parallelism:50, spark.sql.shuffle.partitions:50 and spark.streaming.backpressure.enabled : true
* You can tell the performance of the SparkSession properties by looking at inputRowsPerSecond and processedRowsPerSecond in the Progress Report 