# query account in json
GET logstash-2021.06.21/_search
{
  "query": {
    "match": {
      "json.account": {
        "query" : "SGVO10355_HCM"
      }
    }
  }
}

"hits": {
    "total": 11,
    "max_score": 6.1682153,
    "hits": [
      {
        "_index": "logstash-2021.06.21",
        "_type": "doc",
        "_id": "AXotwk7l4Bm2Gao0IuCC",
        "_score": 6.1682153,
        "_source": {
          "source": "/var/log/custom/channel.json",
          "@timestamp": "2021-06-21T08:47:33.579Z",
          "json": {
            "number": "02873034468",
            "state": "established",
            "direction": "calling",
            "account": "SGVO10355_HCM",
            "peer": "0374322699",
            "duration": 101,
            "connected": 54
          },
          "host": {
            "name": "filebeat"
          },
          "@version": "1",
          "prospector": {
            "type": "log"
          },
          "log": {
            "file": {
              "path": "/var/log/custom/channel.json"
            }
          },
          "input": {
            "type": "log"
          },
          "offset": 71236,
          "tags": [
            "beats_input_raw_event"
          ],
          "beat": {
            "version": "6.8.16",
            "hostname": "filebeat",
            "name": "filebeat"
          }
        }
      },
