# Graphana

---

### Latency Monitoring
Latency is the time it takes for an API call to complete, and it is a critical measure of our service's responsiveness. High latency can signal performance bottlenecks, directly affecting user experience.

There is three key percentile metrics to get a comprehensive view of performance across our API:

- **P75 (75th Percentile)** 🌤️: The experience of most users. This metric shows the point where 75% of API calls were faster than the displayed time. It's a good baseline for general performance.
- **P95 (95th Percentile)** 🌥️: A crucial metric for identifying issues that affect a small but significant portion of our users. It indicates that 95% of requests were completed within this time, helping us spot performance degradation before it becomes a widespread problem.
- **P99 (99th Percentile)** ⛈️: The "worst-case" experience for almost all users. This metric represents the upper limit of our API's response time, showing the point where 99% of calls were faster. Monitoring the P99 is essential for catching and addressing outlier performance issues that can cause significant frustration.
By analyzing these percentile graphs, we can quickly identify trends, detect spikes, and correlate performance issues with specific events like new deployments or traffic surges.


#### Why use percentile to measure performance?
Quote regarding percentile:

>- p50 shows the experience of 50% of the users.
>- p95 shows the experience of 95% of the users. 
>- p99 shows the experience of 99% of the users.

- [Percentile](https://en.wikipedia.org/wiki/Percentile)

- [Response-times-and-what-to-make-of-their-percentile-values](https://www.ombulabs.com/blog/performance/response-times-and-what-to-make-of-their-percentile-values.html)

### Add label to alert
Add label for a better understanding of an alert:
`servicetype {{  index $labels "serviceType.keyword" }} is below {{  $values.C.Value }}  treshold.`

- [Grafana alerting-rules templates](https://grafana.com/docs/grafana/latest/alerting/alerting-rules/templates/)
