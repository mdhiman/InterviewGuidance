

# System Design Core Concepts

## 1. Scalability
- [Horizontal vs Vertical Scaling](https://www.geeksforgeeks.org/scalability-in-distributed-systems/)
- [Load Balancing](https://www.nginx.com/resources/glossary/load-balancing/)
- [Caching Strategies](https://developer.redis.com/explore/cache/cache-strategies/)

## 2. Data Management
- [Database Sharding](https://www.digitalocean.com/community/tutorials/understanding-database-sharding)
- [Replication](https://www.geeksforgeeks.org/replication-in-distributed-system/)
- [Consistency Models](https://jepsen.io/consistency)

## 3. Reliability & Availability
- [CAP Theorem](https://www.geeksforgeeks.org/cap-theorem-in-distributed-systems/)
- [Failover and Redundancy](https://www.ibm.com/docs/en/zos/2.1.0?topic=SSLTBW_2.1.0/com.ibm.zos.v2r1.iean100/iea3n100110.htm)
- [Quorum](https://en.wikipedia.org/wiki/Quorum_(distributed_computing))

## 4. Messaging & Communication
- [Message Queues](https://aws.amazon.com/message-queue/)
- [Publish-Subscribe Pattern](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern)
- [Event-Driven Architecture](https://martinfowler.com/articles/201701-event-driven.html)

## 5. Security
- [Authentication vs Authorization](https://auth0.com/docs/get-started/identity-fundamentals/authentication-and-authorization)
- [Encryption in Transit and at Rest](https://www.cloudflare.com/learning/ssl/what-is-encryption/)
- [Rate Limiting](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After)

## 6. Monitoring & Observability
- [Metrics, Logging, and Tracing](https://opentelemetry.io/docs/concepts/observability/)
- [Health Checks](https://microservices.io/patterns/observability/health-check-api.html)
- [Alerting](https://www.datadoghq.com/solutions/alerting/)

## 7. Design Patterns
- [Microservices](https://martinfowler.com/articles/microservices.html)
- [Monolithic vs Microservices](https://www.geeksforgeeks.org/monolithic-vs-microservices-architecture/)
- [Service Discovery](https://www.nginx.com/learn/service-discovery/)

---

# System Design Research Papers

| S.No | Paper Title | Description | Link |
|------|-------------|-------------|------|
| 1 | Google File System | Google's scalable distributed file system | [PDF](ResearchPaper/GoogleFileSystem.pdf) |
| 2 | MapReduce: Simplified Data Processing on Large Clusters | Google's programming model for processing large data sets | [PDF](ResearchPaper/MapReduce.pdf) |
| 3 | Amazon Dynamo | Highly available key-value store | [PDF](ResearchPaper/amazon-dynamo-sosp2007.pdf) |
| 4 | Cassandra: A Decentralized Structured Storage System | Distributed NoSQL database | [PDF](ResearchPaper/cassandra-decentralized-structured-storage.pdf) |
| 5 | Chubby: Lock Service for Loosely-Coupled Distributed Systems | Distributed lock service by Google | [PDF](ResearchPaper/Chubby-Lock-Sevices.pdf) |
| 6 | Dapper: Large-Scale Distributed Systems Tracing | Distributed tracing infrastructure at Google | [PDF](ResearchPaper/dapper-large-scale-distributed-system-tracing.pdf) |
| 7 | End-to-End Arguments in System Design | Fundamental design principle for distributed systems | [PDF](ResearchPaper/endtoend-systemdesign-argument.pdf) |
| 8 | Bigtable: A Distributed Storage System for Structured Data | Google's distributed storage system | [PDF](ResearchPaper/Google%20Bigtable.pdf) |
| 9 | Kafka: A Distributed Messaging System | Distributed streaming platform | [PDF](ResearchPaper/Kafka.pdf) |
| 10 | LSM-Tree: Log-Structured Merge-Tree | Data structure for write-optimized storage | [PDF](ResearchPaper/LSM-Tee.pdf) |
| 11 | Mesos: Fine-Grained Resource Sharing | Cluster manager for resource sharing | [PDF](ResearchPaper/mesos-finegrained%20resource%20sharing.pdf) |
| 12 | Paxos: The Simple Consensus Algorithm | Consensus protocol for distributed systems | [PDF](ResearchPaper/paxos-simple-Copy.pdf) |
| 13 | Raft: Consensus Protocol | Understandable consensus algorithm | [PDF](ResearchPaper/raft-concensus%20protocol.pdf) |
| 14 | Spanner: Google's Globally Distributed Database | Globally distributed database | [PDF](ResearchPaper/Spanner-Google%20Globally%20Distributed%20Database.pdf) |
| 15 | ZooKeeper: Distributed Coordination Service | Coordination service for distributed applications | [PDF](ResearchPaper/Zookeeper.pdf) |


# Recommended Reading Order for Distributed Systems Papers

---

## **1. Foundational Principles**
Start with the basics to understand the core principles and challenges in distributed systems.

1. **End-to-End Arguments in System Design**  
   *Provides a foundational design principle for distributed systems.*  
   **Reason**: This will give you a strong theoretical foundation to understand why certain design decisions are made in distributed systems.

2. **Paxos: The Simple Consensus Algorithm**  
   *Consensus protocol for distributed systems.*  
   **Reason**: Paxos introduces consensus, a key concept in achieving consistency across distributed nodes.

3. **Raft: Consensus Protocol**  
   *Understandable consensus algorithm.*  
   **Reason**: Raft simplifies Paxos, making it easier to grasp the practical application of consensus in distributed systems.

---

## **2. Distributed Storage Systems**
Learn how distributed systems handle storage, data organization, and scalability.

4. **Google File System**  
   *Google's scalable distributed file system.*  
   **Reason**: It’s the foundation for many distributed storage systems and provides context for Bigtable and MapReduce.

5. **Bigtable: A Distributed Storage System for Structured Data**  
   *Google's distributed storage system.*  
   **Reason**: Builds upon GFS and introduces concepts of columnar storage and indexing.

6. **Amazon Dynamo**  
   *Highly available key-value store.*  
   **Reason**: Dynamo introduces eventual consistency and high availability, which are critical in distributed systems.

7. **Cassandra: A Decentralized Structured Storage System**  
   *Distributed NoSQL database.*  
   **Reason**: Cassandra extends concepts from Dynamo and Bigtable, focusing on scalability and fault tolerance.

8. **LSM-Tree: Log-Structured Merge-Tree**  
   *Data structure for write-optimized storage.*  
   **Reason**: Key for understanding storage engines in systems like Bigtable and Cassandra.

---

## **3. Distributed Coordination and Locking**
Understand how distributed systems coordinate and manage resources.

9. **ZooKeeper: Distributed Coordination Service**  
   *Distributed coordination service.*  
   **Reason**: A practical example of consensus and locking in distributed environments.

10. **Chubby: Lock Service for Loosely-Coupled Distributed Systems**  
    *Distributed lock service by Google.*  
    **Reason**: Complements ZooKeeper and explains Google's approach to resource locking.

---

## **4. Data Processing and Streaming**
Explore how distributed systems process and analyze data.

11. **MapReduce: Simplified Data Processing on Large Clusters**  
    *Google's programming model for processing large data sets.*  
    **Reason**: Essential for understanding distributed data processing.

12. **Kafka: A Distributed Messaging System**  
    *Distributed streaming platform.*  
    **Reason**: Complements MapReduce by introducing real-time data streaming.

---

## **5. Advanced Topics**
Dive into more specialized and advanced areas of distributed systems.

13. **Dapper: Large-Scale Distributed Systems Tracing**  
    *Distributed tracing infrastructure at Google.*  
    **Reason**: Focuses on observability and debugging in distributed systems.

14. **Spanner: Google's Globally Distributed Database**  
    *Globally distributed database.*  
    **Reason**: Extends concepts from Bigtable and Paxos to implement global consistency.

15. **Mesos: Fine-Grained Resource Sharing**  
    *Cluster manager for resource sharing.*  
    **Reason**: Addresses resource sharing and scheduling, a critical aspect of distributed system infrastructure.

---
