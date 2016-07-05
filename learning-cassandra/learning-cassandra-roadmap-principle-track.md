# A Roadmap to Cassandra (The Principle Track)

*Note: This is a preliminary plan, and parts of it may still be under construction.*

## Materials

See [cassandra-resources](https://github.com/hengxin/play-with-cassandra/blob/master/cassandra-resources/cassandra-resources.md) in this project.
## The Cassandra Data Model

### Questions

- How is the data model stored in memory and disk?
- How is the data model different from that in traditional database?
- Give a typical application.

## The Cassandra Architecture: Partition

- Consistent hashing
- Paper [[Chord@SIGCOMM'01]](https://pdos.csail.mit.edu/papers/chord:sigcomm01/chord_sigcomm.pdf): "Chord: A Scalable Peer-to-Peer Lookup Protocol for Internet Applications"

## The Cassandra Architecture: Replication

- Replication strategies

## Read and Write

- Describe the read path and write path.
- How do CommitLog, Memtables, and SSTables work?
- Data structure: Bloom filters
- Data structure: Merkle trees

## Lightweight Transactions (LWT)

- [LWT](http://docs.datastax.com/en/cassandra/3.0/cassandra/dml/dmlLtwtTransactions.html)
