# Timestamp in Cassandra

## Timestamp

- [The trouble with timestamps](https://aphyr.com/posts/299-the-trouble-with-timestamps)

## Vector Clock

- [Does Cassandra use vector clocks](http://grokbase.com/t/cassandra/user/112q75b08y/does-cassandra-use-vector-clocks)

```
NO it does not. 

Instead of using vector clock, it checks the column timestamps.
```

- [CASSANDRA-580: vector clock support](https://issues.apache.org/jira/browse/CASSANDRA-580)

```
Wont Fix.
```

- [DataStax: Why Cassandra doesn¡¯t need vector clocks](https://www.datastax.com/dev/blog/why-cassandra-doesnt-need-vector-clocks)

```
Cassandra avoids the use of vector clocks in favor of finer-grained updates.
```
