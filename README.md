# About
This is a Grafana Loki setup example.

# Running the Example
Run ```docker-compose up```

* Open in browser localhost:3000
* Enter credentials: admin/secret<br>
* Add datasource: 
    * Type:Loki
    * url: http://loki:3100
 * Go to "Explore"
 * Run query: ```{job="varlogs"} |~ "kernel|started"``` 

# Links
* Promtail Pipelines - https://github.com/grafana/loki/blob/master/docs/clients/promtail/pipelines.md
* Loki Compose Guide - https://github.com/grafana/loki/tree/master/production
* LogQL - https://github.com/grafana/loki/blob/master/docs/logql.md
* Grafana Docker User Guide - https://grafana.com/docs/grafana/latest/installation/docker/