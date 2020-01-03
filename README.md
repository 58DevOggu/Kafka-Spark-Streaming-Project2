# Kafka-Spark-Streaming-Project2

Spark Streaming For Project2

##Q1:How did changing values on the SparkSession property parameters affect the throughput and latency of the data?

updating various config values impacted inputRowsPerSecond and processedRowsPerSecond. I could see the increase in throuput and decrease in latency with a few parameter updates

##Q2: What were the 2-3 most efficient SparkSession property key/value pairs? Through testing multiple variations on values, how can you tell these were the most optimal?

when using the default values I got round about 70 processedRowsPerSecond, but when added config like backprrssure enabled in conjunction with high maxOffsetsPerTrigger I got a better throughput of processedRowsPerSecond sometimes peaking at 300
