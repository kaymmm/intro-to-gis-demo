Convert text columns to (long) integers, used to convert census CSV median household income data to usable numeric values:

Pre-logic script code:
```python
import re
def St2Int(theString):
  if (theString == "-"):
    return 0
  theString = re.sub(r"\D", "", theString)
  return int(theString)
```

Field calculator:
```python
St2Int(!fieldname!)
```

