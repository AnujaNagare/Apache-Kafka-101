What Does Kafka Connect Do?

- Kafka Connect is an ecosystem of pluggable connectors, and on the other, a client application
-  As a client application, Connect is a server process that runs on hardware independent of the Kafka brokers themselves.
- It is scalable and fault-tolerant, meaning you can run not just one single Connect worker but a cluster of Connect workers that share the load of moving data in and out of Kafka from and to external systems. 

How Kafka Connect Works
- A Connect worker runs one or more connectors. 
- A connector is a pluggable component that is responsible for interfacing with the external system
-  A source connector reads data from an external system and produces it to a Kafka topic. 
-  A sink connector subscribes to one or more Kafka topics and writes the messages it reads to an external system. 
-  Each connector is either a source or a sink connector, but it is worthwhile to remember that the Kafka cluster only sees a producer or a consumer in either case. 
-  **Everything that is not a broker is a producer or a consumer.**

