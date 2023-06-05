-It would not do if we stored each partition on only one broker. Whether brokers are bare metal servers or managed containers, they and their underlying storage are susceptible to failure, so we need to copy partition data to several other brokers to keep it safe. Those copies are called follower replicas, whereas the main partition is called the leader replica. When you produce data to the leader—in general, reading and writing are done to the leader—the leader and the followers work together to replicate those new writes to the followers.

-This happens automatically, and while you can tune some settings in the producer to produce varying levels of durability guarantees, this is not usually a process you have to think about as a developer building systems on Kafka. All you really need to know as a developer is that your data is safe, and that if one node in the cluster dies, another will take over its role.
