# What Is Apache Kafka?
Apache Kafka is an event streaming platform used to collect, process, store, and integrate data at scale. It has numerous use cases including distributed logging, stream processing, data integration, and pub/sub messaging.


# What Are Events?
An event is any type of action, incident, or change that's identified or recorded by software or applications.

For example, a payment, a website click, or a temperature reading, along with a description of what happened.

# Kafka and Events – Key/Value Pairs
-  Kafka models events as key/value pairs.
-  Kafka famously calls the translation between language types and internal bytes serialization and deserialization. 
-  The serialized format is usually JSON, JSON Schema, Avro, or Protobuf.

- Values are typically the serialized representation of an application domain object or some form of raw message input, like the output of a sensor.
- The key part of a Kafka event is not necessarily a unique identifier for the event, like the primary key of a row in a relational database would be. It is more likely the identifier of some entity in the system, like a user, order, or a particular connected device.
