# Streaming-Data-Analytics

## Understanding User Behavior

A game development company is interested in tracking two events: `buy a sword` & `join guild`.
Each has metadata characterstic of such events (i.e., sword type, guild name, etc).


## Tasks

- Instrument the API server to log events to Kafka
- Assemble the data pipeline to catch these events: use Spark streaming to filter select event types from Kafka, land them into HDFS/parquet to make them
  available for analysis using Presto
- Use Apache Bench to generate test data for your pipeline
- Produce an analytics report where you provide a description of your pipeline and some basic analysis of the events
- Generate and filter more types of events. There are plenty of other things you might capture events for during gameplay
- Enhance the API to use additional http verbs such as `POST` or `DELETE` as well as additionally accept _parameters_ for events (e.g., purchase events might accept sword or item type)
- Connect a user-keyed storage engine such as Redis or Cassandra up to Spark so you can track user state during gameplay (e.g., user's inventory or health)
