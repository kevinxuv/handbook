# 指标监控

指标监控，目前已经成为互联网公司必备的基础运维设施，大部分公司自研或者用开源的解决方案，目前比较流行的开源方案有：

## statsd + graphite + grafana

[statsd](https://github.com/etsy/statsd)，提供指标收集功能，它定义了指标的数据结构。

[graphite](https://graphiteapp.org/) 作为statsd的backend server，用于存储指标数据，并提供查询功能。

[grafana](https://grafana.com/) 是一个时序性数据可视化的组件，是一个非常强大的用来展示时序性数据的前端组件。
