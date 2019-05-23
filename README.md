# Apache Kafka Three Ways: [kafka.troywest.com](http://kafka.troywest.com)

An Open Source Apache Kafka Workshop provided by [Troy-West](http://www.troywest.com), available as a [guided, full day workshop with your team](http://www.troywest.com/workshops).

Project programming materials provided in Java and Clojure :heart_eyes:

Designed to take a full day, this workshop is split into 50% theory and 50% practice.

# Goals

To learn the fundamentals, ergonomics, trade-offs, and maturity of Apache Kafka as:

 1. A Message Broker.
 2. A Streaming Compute Platform.
 3. A Distributed Database.
 
To build a streaming compute system that processes +1M messages and solves the mystery of the Number Stations.

To operate that system in a manner that demonstrates the linear scalability of compute, and trade-offs.

Time permitting, we dabble with vendor tooling (KSQL, Kafka-Connect).

# Prerequisites

* Java 9+ or Clojure & an IDE for completing the Number Stations project work
* [Docker](https://www.docker.com/) & [Docker Compose](https://docs.docker.com/compose/install/) installed
* [troy-west/apache-kafka-cli-tools](https://github.com/troy-west/apache-kafka-cli-tools) cloned
* [troy-west/apache-kafka-number-stations (Java)](https://github.com/troy-west/apache-kafka-number-stations) cloned
* or, [troy-west/apache-kafka-number-stations-clj (Clojure)](https://github.com/troy-west/apache-kafka-number-stations-clj) cloned
* [troy-west/apache-kafka-vendor-tools](https://github.com/troy-west/apache-kafka-vendor-tools) cloned

# Morning Session (Theory)

A deep dive into the history and fundamentals of Apache Kafka as a Message Broker.

We learn about Kafka via the lens of three key project decisions and their trade-offs:

1. High Availability
2. Linear Scalability
3. Near Real-Time Compute

Throughout we focus on real-time data's unifying abstraction, the log.

After the presentation and any Q+A we use [troy-west/apache-kafka-cli-tools](https://github.com/troy-west/apache-kafka-cli-tools) to 
start a local, 3-node Kafka Cluster. We operate that cluster via the shell scripts provided within the Kafka project, 
and observe the impact repartitioning has on a topic.

# Afternoon Session (Practice)



# Self Guided

Start with the index.html in this project, or view at [kafka.troywest.com](http://kafka.troywest.com).

The presentation moves left to right, then vertically for each of the three ways.

Copyright © 2019 Troy-West, Pty Ltd. Released under the MIT license. Contributions welcomed.