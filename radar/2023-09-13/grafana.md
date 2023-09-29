---
title:      "Grafana"
ring:       adopt
quadrant:   tools
tags:       [monitoring, alerting, devops]
---

[Grafana](https://grafana.com/) is an open-source dashboard visualization and alerting software. 
It is an industry standard for this task, and it is written in Go and NodeJS.
It provides a vast choice of different graph types that can be easily combined into dashboards for displaying any kind of numerical or time-based data.

[There is a free repository](https://grafana.com/grafana/dashboards/) of pre-existing dashboards which greatly reduce the time to create new dashboards and alerts. 
It can send alerts via email, Slack, SMS and many more.

In the CHT, Grafana is usually used in conjunction with [Prometheus](https://prometheus.io/) for visualizing both application and infrastructure metrics via the CHT Watchdog.

You can find more details about using Grafana with the CHT Watchdog [in the related documentation](https://docs.communityhealthtoolkit.org/core/overview/watchdog/).
.