# GoSysLab

This repository is a collection of projects and exercises designed to help you learn distributed systems using the Go programming language. It draws inspiration from the [CS425 Distributed Systems course](https://courses.grainger.illinois.edu/cs425/fa2024/lectures.html) offered at the University of Illinois.

## Overview

Distributed systems are at the core of modern computing, enabling scalability, reliability, and fault tolerance. In this repository, we explore key concepts of distributed systems by building practical, project-based examples in Go. Each section corresponds to a set of topics covered in the CS425 lectures, with hands-on projects to reinforce theoretical knowledge.

## Projects

### 1. **Introduction to Distributed Systems**
   - **Topics Covered**: Distributed system models, properties of distributed systems.
   - **Project**: Build a basic client-server communication model using Go's `net` package.
     - Implement a simple TCP-based client-server.
     - Server listens for incoming connections, while clients send messages.

### 2. **Fault Tolerance**
   - **Topics Covered**: Failure models, fault tolerance techniques.
   - **Project**: Implement a heartbeat-based failure detection protocol.
     - Use Goroutines to simulate heartbeats between processes.
     - Detect node failures in a network by monitoring heartbeat timeouts.

### 3. **Consensus Algorithms**
   - **Topics Covered**: Paxos, Raft, leader election.
   - **Project**: Implement the Raft consensus algorithm.
     - Build a distributed key-value store that relies on Raft for state replication.
     - Implement leader election and log replication.

### 4. **Distributed Hash Tables (DHT)**
   - **Topics Covered**: Peer-to-peer systems, Chord protocol.
   - **Project**: Implement the Chord distributed hash table (DHT).
     - Use Go's concurrency features (Goroutines, channels) to create a Chord ring.
     - Simulate nodes joining and leaving the ring and perform lookups using finger tables.

### 5. **MapReduce and Distributed Computation**
   - **Topics Covered**: MapReduce, parallel computation frameworks.
   - **Project**: Build a simplified version of MapReduce in Go.
     - Implement a framework where tasks are distributed across worker nodes to compute results in parallel.

### 6. **Distributed File Systems**
   - **Topics Covered**: Distributed storage, consistency models.
   - **Project**: Implement a distributed file storage system.
     - Simulate distributed file storage with basic consistency models (eventual consistency, strong consistency).
     - Use Go's file handling and concurrency primitives.

### 7. **Failure Detection and Recovery**
   - **Topics Covered**: Failure detection, recovery mechanisms.
   - **Project**: Implement a ring-based failure detection protocol.
     - Use asynchronous message passing between nodes to detect failures.
     - Explore the challenges of false positives and false negatives in failure detection.

### 8. **Quorum-based Systems**
   - **Topics Covered**: Quorum protocols, consistency and availability trade-offs.
   - **Project**: Implement a basic quorum-based voting system.
     - Simulate a distributed database where clients read/write data, and quorum-based voting is used for consistency.

## Prerequisites

- **Go**: You need Go installed on your system. You can download it from [https://golang.org/dl/](https://golang.org/dl/).
- Basic understanding of distributed systems concepts. Refer to the [CS425 lecture notes](https://courses.grainger.illinois.edu/cs425/fa2024/lectures.html) for theoretical background.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/godistributed.git
   cd godistributed
   ```

## Resources

- [CS425 Distributed Systems Course - University of Illinois](https://courses.grainger.illinois.edu/cs425/fa2024/lectures.html)
- [Go Programming Language](https://golang.org/doc/)
