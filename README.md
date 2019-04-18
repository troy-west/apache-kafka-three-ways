# Apache Kafka Three Ways

Apache Kafka Workshop provided by [Troy-West](http://www.troywest.com), presented as a Masterclass at [Voxxed Australia](https://australia.voxxeddays.com/) in May, 2019.

Released under the Apache 2.0 license (the same as Apache Kafka).

Available as a guided, full day workshop with your team. Contact us for details.

Kafka is a database turned inside out, with distribution at heart.
High Availability and Linear Scalability.

Recommend 2.1, due to streaming join semantics (run-ahead, steady-state, protection on stream/table join)

Facts rather than Events
Messages in Kafka have three parts. Key, Value, Timestamp.
Trade-Offs and Knobs to twiddle (max.task.idle.ms for example)

Types of Data:

Mutable v Immutable
Durable v Ephemeral
In Flight v At Rest

Join us for a masterclass on Apache Kafka and Streaming Compute. 

From an overview of Kafka’s nuts and bolts through a practical deep-dive into building real systems, we explore: 

1. Kafka as a Message Broker. 
2. Kafka as a Streaming Compute Platform. 
3. Kafka as a Distributed Database. 

You will learn where Apache Kafka has come from, how it works, what problem it addresses, when it is suitable to, adopt, and where it is headed. 

We demonstate scalability, availability, domain modelling, semantic partitioning,the consume-transform-produce idiom, basic operations, the Kafka Streams DSL, when to use the Processor API, local, state, idempotence, immutability, and most importantly how to build real systems that leverage Apache Kafka correctly.

Full Day - 4 Sections (80 mins each)
The masterclass will be divided into 4 sections of around 80 minutes each. Each section should provide individual objectives and takeaways. The following will outline these, the delivery methods and a timeline for each section.

Rather than do one big lecture at the start of the day we will give a shorter 10-15 minute presentation on Kafka architecture at the start of each of the 4 sections. Each presentation should seek to provide context for the practical exercises and build on the knowledge obtained from the previous section. This should serve to break up the day and get attendees engaged and interacting as quickly as possible.

Major Motivations: Linear Scalability (Data / Compute), High Availability, Data-Oriented (Logs!)
Section 1 - Kafka as a Message Broker
Objectives
Provide an overview of the Kafka architecture, discussing the unifying log abstraction that Kafka is built on. Understand how to use Kafka as message broker and what the benefits and trade-offs of doing so compared to RabbitMQ/SQS/JMS.. Get hands on experience using a Kafka cluster to broker messages between consumers and producers.
Topics to be covered
The Log
Replication
Determinism
Ordering changes and distributing data
Message Broker
Brokers
Topics
Consumers
Push Vs Pull
Consumer Offsets
Producers
Semantic partitioning
Load balancing
Delivery Semantics
Strong Durability
Time-To-Live
Fault Tolerance
Partitioning
Data locality
Takeaways
Attendees should be able to:
Identify the attributes that make Kafka a good message broker. 
Describe what a Kafka topic is.
Spin up a multi-node Kafka cluster for testing using Docker.
Use Kafka consumers and producers to read and write message to and from a topic.
Understand the basics of consumer offsets.
Use consumers to read from a point in time.
Understand the importance of time-to-live when using Kafka as message broker.
Be able to describe the delivery semantics of Kafka.
Delivery
Slide show presentation.
Interactive tutorial used Docker containers and Kafka CLI tools.
BeakerX notebook to write code to read/write messages using consumers/producers.
Timeline

5 min - Introduction & Setup
Who are we?
What can you expect to take away from the masterclass?
Outline of the masterclass.
What can you expect to take away from this section?
What tools will we be using?
Installation instructions.
Start downloads and installation now!

5 mins - Presentation: The Log, Kafka’s central abstraction
20 mins - Presentation: Kafka as a Message Broker
50 mins - Practical: Using consumers and producers
Section 2 - Kafka as a Streaming Compute Platform
Objectives
Explore Kafka’s ability to compute over large volumes of data. Understand benefits and trade-offs compared to Storm/Flink.
Topics to be covered
Data Integration
ETL
Consume-transform-produce
Scalability
Semantic Partitioning
Idempotence, Immutability and Replay
Kafka Streams
Topologies
Streams DSL
Windowing
Processor API (PAPI)
KSQL
Local State
RocksDB
Materialized Stores
Takeaways
Attendees should be able to:
Write a small Kafka streams topology use the Streams DSL.
Write a topology using the PAPI, storing state in RockDB tables.
Write tests a for streams topology against the Kafka streams test driver.
Understand how to scale a Kafka streams compute application, running many processes in parallel.
Delivery
Slide show presentation.
Interactive tutorial using BeakerX and the Kafka streams test driver.
Exercises using an IDE and Docker containers.
Timeline

2 mins - Presentation: Recap
8 mins - Presentation: Kafka as a Streaming Compute Platform
50 mins - Practical: Writing a streaming topology
15 mins - Streams DSL
15 mins - Windowing
25 mins - PAPI

10 mins - PresentationPractical: Deploying a streaming application
Section 3 - Kafka as a Distributed Database
Objectives
Understand how Kafka can be used to a distributed database, serving application queries. To give a framework for understanding how and why domain modelling is different in this context than in traditional relational databases. To give practical, actionable knowledge on how to use Kafka as a database and implement an application to perform interactive queries.
Topics to be covered
Changelog
Table and Event Duality
Materialized Views
Domain Modelling
Joining Streams
Interactive Queries
Takeaways
Attendees should be able to:
Implement a web server to serve interactive queries from a Kafka cluster.
Understand the need for identifying read paths when modelling data.
Delivery
Slide show presentation.
Exercises using an IDE and Docker containers.
Timeline

2 mins - Presentation: Recap
8 mins - Presentation: Kafka as a Distributed Database
10 mins - Practical: Setup project in IDE
60 mins - Practical: Putting it all together
20 mins - Making a materialized view
40 mins - Building an application to perform interactive queries

Section 4 - Kafka Connect and KSQL

Objectives
Topics to be covered
Takeaways
Attendees should be able to:
Delivery
Timeline


Copyright © 2019 Troy-West, Pty Ltd.
