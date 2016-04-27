# stream-manager
A library for managing typed streams. Built on top of Avro, Kafka, and Apache Spark. Usage:
```
import com.parachutebilling.StreamManager

StreamManager.addStream("MyStream", "MyTopic", "MyType")
val df: org.apache.spark.sql.DataFrame = StreamMamager.toDataFrame("MyStream")
```
