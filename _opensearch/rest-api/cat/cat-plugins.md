---
layout: default
title: cat plugins
parent: CAT
grand_parent: REST API reference
nav_order: 50
has_children: false
---

# cat plugins

The cat plugins operation lists the names, components, and versions of the installed plugins.

## Example

```
GET _cat/plugins?v
```

## Path and HTTP methods

```
GET _cat/plugins
```

## URL parameters

All cat plugins URL parameters are optional.

In addition to the [common URL parameters]({{site.url}}{{site.baseurl}}/opensearch/rest-api/cat/index#common-url-parameters), you can specify the following parameters:

Parameter | Type | Description
:--- | :--- | :---
local | Boolean | Whether to return information from the local node only instead of from the master node. Default is false.
master_timeout | Time | The amount of time to wait for a connection to the master node. Default is 30 seconds.


## Response

```json
name       component                       version
odfe-node2 opendistro-alerting             1.13.1.0
odfe-node2 opendistro-anomaly-detection    1.13.0.0
odfe-node2 opendistro-asynchronous-search  1.13.0.1
odfe-node2 opendistro-index-management     1.13.2.0
odfe-node2 opendistro-job-scheduler        1.13.0.0
odfe-node2 opendistro-knn                  1.13.0.0
odfe-node2 opendistro-performance-analyzer 1.13.0.0
odfe-node2 opendistro-reports-scheduler    1.13.0.0
odfe-node2 opendistro-sql                  1.13.2.0
odfe-node2 opendistro_security             1.13.1.0
odfe-node1 opendistro-alerting             1.13.1.0
odfe-node1 opendistro-anomaly-detection    1.13.0.0
odfe-node1 opendistro-asynchronous-search  1.13.0.1
odfe-node1 opendistro-index-management     1.13.2.0
odfe-node1 opendistro-job-scheduler        1.13.0.0
odfe-node1 opendistro-knn                  1.13.0.0
odfe-node1 opendistro-performance-analyzer 1.13.0.0
odfe-node1 opendistro-reports-scheduler    1.13.0.0
odfe-node1 opendistro-sql                  1.13.2.0
odfe-node1 opendistro_security             1.13.1.0
```
