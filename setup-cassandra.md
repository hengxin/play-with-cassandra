# Setup Cassandra

## Install and Run Locally

### From [DataStax](https://academy.datastax.com/downloads/welcome)
*Note: It does not use the latest version of Cassandra.*

### From Tarball

1. Download cassandra
- [cassandra](http://cassandra.apache.org/download/)
  
  Official Apache Cassandra.
- [planetcassandra](http://www.planetcassandra.org/cassandra/)

  Including both the official Apache Cassandra and some vendor-provided Cassandra distributions, 
  like DataStax Distribution of Apache Cassandra (DDC), Stratio Cassandra, and DataStax Enterprise.
  
  > We choose the DataStax Distribution. As of writing, it is `datastax-ddc-3.5.0-bin.tar.gz`.
  
2. Unzip
`tar -xvzf datastax-ddc-3.5.0-bin.tar.gz`

3. Run cassandra
`bin/cassandra -f`

4. Run cqlsh
`bin/cqlsh`

### Build from Sources
