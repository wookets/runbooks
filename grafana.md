
# Grafana

## Queries

Metrics per second

```promql
sum by(prometheus) (sum_over_time(scrape_samples_scraped[5m]) / 300)
```

Look for a pod via regex.

```promql
{pod=~"podn.*"}
```
