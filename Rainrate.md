```yaml
type: custom:apexcharts-card
header:
  title: PWS - Rainrate
  show: true
  standard_format: true
  show_states: true
apex_config:
  chart:
    height: 300px
  yaxis:
    tickAmount: 5
graph_span: 8d
span:
  start: day
  offset: '-7d'
stacked: true
series:
  - entity: sensor.pws_rainrate
    name: Rainrate
    type: line
    curve: stepline
```
