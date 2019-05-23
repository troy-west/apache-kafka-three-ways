# Apache Kafka Three Ways: [(kafka.troywest.com)]
## Online @ http://kafka.troywest.com

An Open Source Apache Kafka Workshop provided by [Troy-West](http://www.troywest.com), available as a [guided, full day workshop with your team](http://www.troywest.com/workshops).

Project programming materials provided in Java and Clojure :heart_eyes:

Designed to take a full day, this workshop is split into 50% theory and 50% practice.

# Goals

To learn the fundamentals, ergonomics, trade-offs, and maturity of Apache Kafka as:

 1. A Message Broker.
 2. A Streaming Compute Platform.
 3. A Distributed Database.
 
To build a streaming compute application that processes +1M messages and solves the mystery of the Number Stations.

To operate the streaming compute application with a local Kafka cluster, understanding the tiered abstractions of Apache Kafka and how they enable availability, scalability, and (near) real-time compute.

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
start a local, 3-node Kafka Cluster. We operate that cluster via the shell scripts by Kafka, exploring repartitioning, offsets, consumer groups, and more.

# Afternoon Session (Practice)

#### Solve the mystery of the Numbers Stations!

After a shorter presentation on the big ideas behind the Processor API and Kafka Streams we dig into 
[troy-west/apache-kafka-number-stations](https://github.com/troy-west/apache-kafka-number-stations) (or the Clojure variant).

We look at the output of the secret radio, send 1.5M messages to local Kafka, then progressively fix unit-tests as we
build a streaming compute application that filters, branches, maps, groups, windows, and aggregates data until we have
decoded the secret message. 

Once the tests are green we build and deploy multiple versions of the system, discussing the expected and observed impact
on local state / message decoding. The partitioning of data through topics to k-tables writ large.

Finally we discuss Interactive Queries and the possibility of using Kafka as a distributed database. What data should we expect to source from Kakfa, just the logs, or derived / materialized / computed data? 

# Self Guided

Start with the index.html in this project, or view at [kafka.troywest.com](http://kafka.troywest.com).

The presentation moves left to right, then vertically for each of the three ways.

Copyright © 2019 Troy-West, Pty Ltd. Released under the MIT license. Contributions welcomed.