# hive-metastore

## Setup

### Usage

```bash
$ git clone https://github.com/ozkatz/hive-metastore
$ cd hive-metastore
```
And then run

```bash
$ export S3_BUCKET="my-bucket"
$ export S3_PREFIX="path/to/warehouse/"
$ docker compose up
```

You can now connect to the MetaStore Thrift server at `0.0.0.0:9093` from your host machine.

### Configuration

Controlled via ENVironment variables

Key                | Required?                             | Description
-------------------|---------------------------------------|-------------
S3_BUCKET          | Yes                                   | S3 bucket name
S3_PREFIX          | Yes                                   | S3 bucket prefix

make sure to export both before running.