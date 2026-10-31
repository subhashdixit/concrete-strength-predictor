# Feature contract

All named columns are required in CSVs. A blank value means missing; extra columns are ignored. Defaults are synthetic training medians/modes. Numeric bounds constrain serving and mark unsupported source values missing during training. They do not define a population validity guarantee.

| Source field | Meaning / units | Accepted values |
|---|---|---|
| `cement` | cement (kg/m³) | 0 to 2000 |
| `slag` | slag (kg/m³) | 0 to 2000 |
| `fly_ash` | fly ash (kg/m³) | 0 to 2000 |
| `water` | water (kg/m³) | 0 to 2000 |
| `superplasticizer` | superplasticizer (kg/m³) | 0 to 2000 |
| `coarse_aggregate` | coarse aggregate (kg/m³) | 0 to 2000 |
| `fine_aggregate` | fine aggregate (kg/m³) | 0 to 2000 |
| `age` | Curing age (days) | 1 to 365 (whole numbers) |
