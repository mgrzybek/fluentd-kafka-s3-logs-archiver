# fluentd-kafka-s3-logs-archiver

Fluentd container using Kafka as input and S3 as output

This custom image is inspired by the [official repository](https://github.com/fluent/fluentd-docker-image).

## Usage

The following environment variables are to be set:

```
broker_servers
consumer_group
topics
max_bytes
max_wait_time
min_bytes
offset_commit_interval
offset_commit_threshold
fetcher_max_queue_size
refresh_topic_interval
start_from_beginning
access_key
secret_key
bucket_name
endpoint
region
path
timekey
timekey_wait
timekey_use_utc
chunk_limit_size
```

Please refer to the official:

- [kafka documentation](https://github.com/fluent/fluent-plugin-kafka#input-plugin-type-kafka_group-supports-kafka-group)
- [s3 documentation](https://github.com/fluent/fluent-plugin-s3/blob/master/docs/input.md)
