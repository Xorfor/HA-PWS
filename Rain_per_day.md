# Rain per day
To display the amount of rain per day.

## Configuration
```yaml
type: custom:apexcharts-card
graph_span: 8d
span:
  start: day
  offset: '-7d'
header:
  show: true
  title: PWS - Rain
  standard_format: true
  show_states: true
series:
  - entity: sensor.pws_rain
    type: column
    group_by:
      func: max
      duration: 1d
```

## Screenshot
![Screenshot](images/rain_per_day.jpg)
