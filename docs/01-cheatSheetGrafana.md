# Graphana

---

- Alert summary:
```jsx
servicetype {{  index $labels "serviceType.keyword" }} is below {{  $values.C.Value }}  treshold.
```
[Grafana alerting-rules templates](https://grafana.com/docs/grafana/latest/alerting/alerting-rules/templates/)
