### Python REST Framework
[Django URLs](https://docs.djangoproject.com/en/1.11/topics/http/urls/#example)
[more info](http://www.django-rest-framework.org/#example)

### Rails resources
[more info](http://guides.rubyonrails.org/routing.html#resource-routing-the-rails-default)

```ruby
# config/routes.rb
root 'posts#index'
resources :posts
```
```shell
$ rails routes
   Prefix Verb   URI Pattern               Controller#Action
     root GET    /                         posts#index
    posts GET    /posts(.:format)          posts#index
          POST   /posts(.:format)          posts#create
 new_post GET    /posts/new(.:format)      posts#new
edit_post GET    /posts/:id/edit(.:format) posts#edit
     post GET    /posts/:id(.:format)      posts#show
          PATCH  /posts/:id(.:format)      posts#update
          PUT    /posts/:id(.:format)      posts#update
          DELETE /posts/:id(.:format)      posts#destroy
```
