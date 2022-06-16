## Go to site:
https://dev.to/elastic/downloading-elasticsearch-and-kibana-macos-linux-and-windows-1mmo

## Save both elasticsearch and kibana need to be in same root folder
1) Download Elasticsearch
2) Download Kibana

## Running ELASTICSEARCH
3) cd to root folder (project folder)
4) cd/elasticsearch-<version>
5) run elastic search
```
bin/elasticsearch

```
6) cd config/elasticsearch.yml 
- update security setting  from true to false
```
xpack.security.enabled: false
```
7) run curl command to test connection

```
curl http://localhost:9200
```
-should return response
```
{
  "name" : "jimmys-mbp-2.lan",
  "cluster_name" : "elasticsearch",
  "cluster_uuid" : "uuid information here",
  "version" : {
    "number" : "8.2.3",
    "build_flavor" : "default",
    "build_type" : "tar",
    "build_hash" : "9905bfb62a3f0b044948376b4f607f70a8a151b4",
    "build_date" : "2022-06-08T22:21:36.455508792Z",
    "build_snapshot" : false,
    "lucene_version" : "9.1.0",
    "minimum_wire_compatibility_version" : "7.17.0",
    "minimum_index_compatibility_version" : "7.0.0"
  },
  "tagline" : "You Know, for Search"
}
```
## RUNNING KIBANA
8) cd to root folder (project folder)
4) cd/kibina
5) run kibana
```
bin/kibana

```
6) open in browser to http://localhost:5601
7) go to Dev Tools 