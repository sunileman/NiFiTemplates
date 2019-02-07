# NiFiTemplates
NiFi Templates

HTTP_payload <br>
Generates flow file with a payload (any type you which).  Push data to rest end point (listenHTTP endpoint) using gzip compression
Another flow has ListenHTTP which then decompresses payload, merge content (to make larger payload), and push to HDFS


NiFi_Benchmark <br>
Workflow designed to benchmark your cluster.  If you want push your cluster limits add more activity (processors) to the template

Log_Parsing.xml <br>
Workflow designed to ingest unstructured logs (ie windows) and parse them via grok.  The output of the parsing is a json structure which can be sinked to virtually any target.



Hive3Streaming.xml <br>
Workflow designed to generate json data and stream into Hive3

SplitJsonArray.xml <br>
Workflow designed to generate json array (7 records), split into indivdual json records, pull a attribute from the json event and route on it


MiNiFi_Demo.xml <br>
In this template, there are two main process group. One for NiFi and other for MiNiFi flow.  The MiNiFi flow has also bee seperated in another flow called MiNiFi_Flow.xml


MiNiFi_Flow.xml <br>
This flow resides in MiNiFi.  It generates sensor data and exposes end point for end users to send instructions to


