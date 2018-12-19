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
