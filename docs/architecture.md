# Architecture

## Components

### Client

Sends GET, SET, and DELETE requests.

### Leader Node

Handles client write requests and coordinates replication.

### Follower Nodes

Replicate log entries and maintain consistency.

### Storage Layer

Stores key-value data and write-ahead logs.

### Consensus Layer

Implements Raft-based leader election and log replication.

## High-Level Flow

Client
→ Leader
→ Followers
→ Majority Acknowledgement
→ Commit
→ Response
