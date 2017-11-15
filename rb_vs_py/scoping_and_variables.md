### Python Variables
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

### Ruby Variables
| ---               | ---         | --- |
| Global            | $dollar     | Global in every scope, caution |
| Constant          | ALL_CAPS    | Always accessable with prefixes |
| Class variable    | @@double_at | Only accessable to defining class and any subclasses |
| Instance variable | @single_at  | Only accessable within the object or through getter methods |


### Python arguments
```py
class ThingDoer():
  __init__(self, more_things):
    self.things = ['thing1','thing2',more_things]
def do_things(arg, extra_kwarg=False, *args, **kwargs):
  # args is a list
  # kwargs is a dict
  super().do_things(*args, **kwargs) # re-pack args and kwargs
```

### Ruby arguments
```ruby
class ThingDoer
  def initialize more_things
    @things = ['thing1']
  end
end
def do_things(*args, a: true, b: false)
  # args is an array
end
```
[more info](http://codeloveandboards.com/blog/2014/02/05/ruby-and-method-arguments/)
