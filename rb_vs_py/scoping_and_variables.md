### Python
| ---    | --- |
| Global | All top-level variables are global to the module they are defined in. |
| Local  | Variables defined in methods or classes are not available outside. |

```py
# dennis.py
name = "Dennis"

# gretting.py
from '.dennis' import name as dennis_name
print(dennis_name) # Yep
```

### Ruby
| ---               | ---         | --- |
| Global            | $dollar     | Global in every scope, caution |
| Constant          | ALL_CAPS    | Always accessable with prefixes |
| Class variable    | @@double_at | Only accessable to defining class and any subclasses |
| Instance variable | @single_at  | Only accessable within the object or through getter methods |
