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
