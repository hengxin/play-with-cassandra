# Fork Apache Cassandra

The document shows how to fork Apache Cassandra locally and keep it up-to-dated.
The following steps are borrowed from [this blog: Reading Spark Souce Code in IntelliJ
IDEA](http://linbojin.github.io/2016/01/09/Reading-Spark-Souce-Code-in-IntelliJ-IDEA/).

1. Fork Apache Cassandra to your own GitHub account.

2. Clone Apache Cassandra to your local host from your own GitHub account.

```
git clone https://github.com/YOUR-USER-NAME/cassandra.git
cd cassandra/
```

3. Add remote to Apache Cassandra

```
git remote add apache https://github.com/apache/cassandra.git
```

4. Sync repository with Apache Cassandra

```
git fetch apache
git pull apache trunk
```

5. Push new updates to your own github account repo:

```
git push origin master
```
