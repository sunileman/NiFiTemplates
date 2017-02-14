# NiFiTemplates
NiFi Templates

HTTP_payload.xml
Generates flow file with a payload (any type you which).  Push data to rest end point (listenHTTP endpoint) using gzip compression
Another flow has ListenHTTP which then decompresses payload, merge content (to make larger payload), and push to HDFS

