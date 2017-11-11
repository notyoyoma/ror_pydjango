
#### Itteration
```py
# Python comprehensions
list = [1,2,3]
print(x) for x in list```
```rb
# Ruby blocks
[1,2,3].each { |x| puts x }
# or
[1,2,3].each do |x|
  puts x
end
```
Ruby also has lambdas and procs, that can do similar things. [More Info](http://awaxman11.github.io/blog/2013/08/05/what-is-the-difference-between-a-block/)

#### Store results
```py
# Python comprehensions
list = [1,2,3]
list2 = [x*2 for x in list]```
```rb
# Ruby blocks
[1,2,3].collect { |x| puts x*2 }
# or
[1,2,3].collect do |x|
  puts x*2
end
```
[More Ruby Ennmerable Methods](https://ruby-doc.org/core-2.2.3/Enumerable.html)

## Cheat Sheet
[Hyperpolyglot Cheat Sheet](http://hyperpolyglot.org/scripting)
| rb | py |
| -- | -- |
| [1,2,3].all? {&#124;x&#124; x>0}        | all(x>0 for x in [1,2,3])|
| [1,2,3].find_all {&#124;x&#124; x%2==0} | [x for x in [1,2,3] if x%2==0]|
