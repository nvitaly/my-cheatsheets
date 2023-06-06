


#### Saving pandas dataframes to exel

```python
import pandas as pd

# data is dictionary of dataframes

writer = pd.ExcelWriter('capacity_test.xlsx', engine='xlsxwriter')
for report in data:
    data[report].to_excel(writer, sheet_name=report, index=False)
writer.close()
```



