---
title:      "Grafana"
ring:       adopt
quadrant:   tools
tags:       [monitoring, alerting, devops]
---

<a href="https://grafana.com/">Grafana</a> is an open-source dashboard visualization and alerting software. 
It is an industry standard for this task, and it is written in Go and NodeJS.
It provides a vast choice of different graph types that can be easily combined into dashboards for displaying any kind of numerical or time-based data.

<a href="https://grafana.com/grafana/dashboards/">There is a free repository</a> of pre-existing dashboards which greatly reduce the time to create new dashboards and alerts. 
It can send alerts via email, Slack, SMS and many more.

In the CHT, Grafana is usually used in conjunction with <a href="https://prometheus.io/">Prometheus</a> for visualizing both application and infrastructure metrics via the CHT Watchdog.

You can find more details about using Grafana with the CHT Watchdog
<a href="https://docs.communityhealthtoolkit.org/core/overview/watchdog/">in the related documentation</a>.