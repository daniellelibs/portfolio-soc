# Splunk SOC Lab - Week 1

5 core SPL queries for SIEM analysis.

## Queries

See `queries/01-basic-queries.spl`

1. Basic search: `index=_internal | head 10`
2. Filter source: `index=_internal source=*splunkd.log*`
3. Stats: `index=_internal | stats count by host`
4. Boolean OR: `index=_internal (source=*splunkd.log* OR source=*metrics.log*)`
5. Timechart: `index=_internal | timechart count by source`

## Screenshots

See `screenshots/` folder

---

Author: Libiane Souza
Date: October 6, 2024
