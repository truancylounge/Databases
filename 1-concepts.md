# Database Concepts

## Distributed databases concepts
- https://www.dragonflydb.io/blog/modern-distributed-database-architectures-part-01
- https://www.dragonflydb.io/blog/modern-distributed-database-architectures-part-02
- **Consistent Hashing**:
  - It's a distributed hashing technique used in load balancing or distributed databases. The goal is to minimize the need for rehasing when number of nodes in system changes
  - Issues with Traditional Hashing methods:
    - Uneven distribution of data
    - Scalability Problems
    - Inflexibility with Changing number of servers
    - Node failure handling
    - Overhead of Rehashing
  - Consistent hashing solves these issues, https://www.geeksforgeeks.org/system-design/consistent-hashing/
- **Layered Architecture** vs **Primary Replica Model** vs **Shared-nothing Architecture**
- **Two-Phase Commit**, in distributed algorithm ensures all nodes in distributed databse either commit or abort a transaction. 
  - **Prepare Phase (Voting)**, where coordinator asks participants if they are ready to commit ("yes" or "no")
  - **Commit/Rollback Phase (Decision)**, If all participants vote "yes", coordinator sends **"COMMIT"** message to everyone, else "**ABORT**"(rollback) message.
  - Locks are placed until COMMIT or ABORT is received by each node
-  


## Resources:
1. https://www.geeksforgeeks.org/system-design/consistent-hashing/
2. 