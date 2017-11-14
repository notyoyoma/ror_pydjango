### Django Static
```html
{% load static %}
<img src="{% static "my_app/example.jpg" %}" alt="My image"/>
```


### Rails Asset Pipeline
```html
<head>
  <%= stylesheet_link_tag    'application', media: 'all' %>
  <!-- application.[s]css -->
  <%= javascript_include_tag 'application' %>
  <!-- application.js -->
</head>
<body>
  <%= image_tag "rails.png" %>
</body>
```
[more info](http://edgeguides.rubyonrails.org/asset_pipeline.html#coding-links-to-assets)
```scss
.body {
  background: image-url("rails.png");
}
```
[more info](http://edgeguides.rubyonrails.org/asset_pipeline.html#css-and-sass)
```js
$('#logo').attr({ src: "<%= asset_path('logo.png') %>" });
```
[more info](http://edgeguides.rubyonrails.org/asset_pipeline.html#javascript-coffeescript-and-erb)
