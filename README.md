tCouchbaseBulk
==============

Talend component to convert and push json documents to couchbase server.

Prereqs
=============

- Talend Open Studio for Data Integration (5.2.1 or above)

- tCouchbaseConnection: (https://github.com/ronniedada/tCouchbaseConnection) 

    A predefined connection connects to couchbase server.

- A directory of json documents on your local computer.

Settings
=============

- Connection: tCouchbaseConnection component which handles the connection to couchbase server. 

- Path: absolute path which contains the json docuements to load.

- Batch: number of documents to check for server ACKs before sending new ones.

Limitations
=============

- Current implementations support flat directory strucuture only, i.e: subdirectories will be bypassed with a returned error.

- Does not recognize couchbase cluster change.

 
