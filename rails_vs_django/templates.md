### Django Templates
[More Info on Jinja](http://jinja.pocoo.org/)

```py
# views.py
class PostView(views.ModelView):
  def get_context_data(self, *args, **kwargs):
    context = super().get_context_data(*args, **kwargs)
    context['new_data'] = "Hello World"
```
```html
<!-- template.html -->
<h1>{{ new_data }}</h1>
```

In Django, all data must be passed into the template through the *context* variable. You can also write custom [templatetags](https://docs.djangoproject.com/en/1.11/howto/custom-template-tags/) that transform the data. However, these only have access to the data provided in *context*.

### Rails Templates
```ruby
# posts_controller.rb
class PostsController < ApplicationController
  def index do
    @new_data = "Hello World"
  end
```
```html
<h1><%= new_data %></h1>
```

#### A major difference
In Rails, you can run new queries in views. For example:
```html
<ul>
  <% Post.all.each do |post| %>
    <li><%= post.title %></li>
  <% end %>
</ul>
```
This can be very inneficient, but it can also be very nice.
