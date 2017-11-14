### Importing Modules
Very Similar:
```py
#python
import 'requests'
```
```rb
# ruby
require 'net/http'
```

### Alias a module method in the local scope
```py
# python import as
from 'requests' import get as http_get
http_get(...)
```
```rb
# ruby require and alias
require 'net/http'
http_get = Net::HTTP.get
http_get(...)
```

### Importing config files
```py
# python
from yaml import load, CLoader as Loader
data = load(open('filename.yml'), Loader=Loader)
```
```py
# ruby
require 'yaml'
data = YAML.load_file('filename.yml')
```

### Inheritance
```py
# python
class Parent:
  pass

class Child(Parent):
  pass
```
```ruby
# ruby
class Parent
end

class Child < Parent
end
```

### Multiple Inhretiance
```py
#python
class Parent1:
  pass

class Parent2:
  pass

class Child(Parent1, Parent2):
  pass
```

If you have a class that is only intended to be included in other classes, end it with *Mixin*. (`OtherMethodsMixin`)

```ruby
# ruby extend and include
class Parent
end

module OtherMethods
  def do_things
  end
end

class Child1 < Parent
  extend OtherMethods #Attaches methods to class
end

class Child2 < Parent
  include OtherMethods #Attaches methods to instance
end
```
