# PySpark_1

The initial repository for all PySpark usage projects.   
Am using a Local Setup of Spark   
```
Spark 2.0.2 built for Hadoop 2.7.3

```
#

1. Daily Show Data ~ followed the DataQuest tutorials
#
2. Collating Best Practices for analysing Large data Sets  
#
2.1 
#
2.2
#
2.3 
#
#
#
Confusing Examples from the Net :- 

a/ PySpark first approaches. Tips and tricks  

Posted on August 28, 2016  
Author -- Elena Cuoco URL --- https://www.elenacuoco.com/2016/08/28/pyspark-first-approaches-ml-classification/  
The Author states she had access to a 17 Core 16GbRAM in which she couldnt load the Train CSV 
for the Bosch Kaggle competition .   
She seems to have loaded that in STANDALONE mode in Spark 2.0  
Need to understand further !!

#
b/

#
More refrences from the net --   
#
a/ https://www.elenacuoco.com/2016/09/01/pyspark-for-redhat-kaggle-competition/






#### incase you leave a local Spark running overnight ...

```
17/08/31 10:16:10 WARN HeartbeatReceiver: Removing executor driver with no recent heartbeats: 72740841 ms exceeds timeout 120000 ms
17/08/31 10:16:15 ERROR TaskSchedulerImpl: Lost executor driver on localhost: Executor heartbeat timed out after 72740841 ms
17/08/31 10:16:23 WARN NettyRpcEnv: Ignored message: true
17/08/31 10:16:23 WARN NettyRpcEndpointRef: Error sending message [message = Heartbeat(driver,[Lscala.Tuple2;@32a17def,BlockManagerId(driver, 192.168.0.100, 34841))] in 1 attempts
org.apache.spark.rpc.RpcTimeoutException: Futures timed out after [10 seconds]. This timeout is controlled by spark.executor.heartbeatInterval
	at org.apache.spark.rpc.RpcTimeout.org$apache$spark$rpc$RpcTimeout$$createRpcTimeoutException(RpcTimeout.scala:48)
	at org.apache.spark.rpc.RpcTimeout$$anonfun$addMessageIfTimeout$1.applyOrElse(RpcTimeout.scala:63)
	at org.apache.spark.rpc.RpcTimeout$$anonfun$addMessageIfTimeout$1.applyOrElse(RpcTimeout.scala:59)
	at scala.PartialFunction$OrElse.apply(PartialFunction.scala:167)
	at org.apache.spark.rpc.RpcTimeout.awaitResult(RpcTimeout.scala:83)
	at org.apache.spark.rpc.RpcEndpointRef.askWithRetry(RpcEndpointRef.scala:102)
	at org.apache.spark.executor.Executor.org$apache$spark$executor$Executor$$reportHeartBeat(Executor.scala:518)
	at org.apache.spark.executor.Executor$$anon$1$$anonfun$run$1.apply$mcV$sp(Executor.scala:547)
	at org.apache.spark.executor.Executor$$anon$1$$anonfun$run$1.apply(Executor.scala:547)
	at org.apache.spark.executor.Executor$$anon$1$$anonfun$run$1.apply(Executor.scala:547)
	at org.apache.spark.util.Utils$.logUncaughtExceptions(Utils.scala:1953)
	at org.apache.spark.executor.Executor$$anon$1.run(Executor.scala:547)
	at java.util.concurrent.Executors$RunnableAdapter.call(Executors.java:511)
	at java.util.concurrent.FutureTask.runAndReset(FutureTask.java:308)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.access$301(ScheduledThreadPoolExecutor.java:180)
	at java.util.concurrent.ScheduledThreadPoolExecutor$ScheduledFutureTask.run(ScheduledThreadPoolExecutor.java:294)
	at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1142)
	at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:617)
	at java.lang.Thread.run(Thread.java:745)
Caused by: java.util.concurrent.TimeoutException: Futures timed out after [10 seconds]
	at scala.concurrent.impl.Promise$DefaultPromise.ready(Promise.scala:219)
	at scala.concurrent.impl.Promise$DefaultPromise.result(Promise.scala:223)
	at scala.concurrent.Await$$anonfun$result$1.apply(package.scala:190)
	at scala.concurrent.BlockContext$DefaultBlockContext$.blockOn(BlockContext.scala:53)
	at scala.concurrent.Await$.result(package.scala:190)
	at org.apache.spark.rpc.RpcTimeout.awaitResult(RpcTimeout.scala:81)
	... 14 more
17/08/31 10:16:25 WARN SparkContext: Killing executors is only supported in coarse-grained mode
17/08/31 10:16:23 WARN NettyRpcEnv: Ignored message: HeartbeatResponse(true)
```

