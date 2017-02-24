# NiFiTemplates
NiFi Templates

HTTP_payload
Generates flow file with a payload (any type you which).  Push data to rest end point (listenHTTP endpoint) using gzip compression
Another flow has ListenHTTP which then decompresses payload, merge content (to make larger payload), and push to HDFS


NiFi_Benchmark
Workflow designed to benchmark your cluster.  If you want push your cluster limits add more activity (processors) to the template
