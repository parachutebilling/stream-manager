# stream-manager
A library for managing typed streams. Built on top of Avro, Kafka, and Apache Spark. Usage:
```
import com.parachutebilling.StreamManager

StreamManager.addSqlContext(sqlContext)
StreamManager.addTypeTopic("Type")    // "Type" is default
StreamManager.init

StreamManager.addStream("MyStream", "MyTopic", "MyType")
val df: org.apache.spark.sql.DataFrame = StreamMamager.toDataFrame("MyStream")
```
