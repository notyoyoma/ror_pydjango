```bash
rails generate scaffold NAME [field[:type][:index] field[:type][:index]] [options]
```

Example:
```bash
rails g scaffold Post title:string content:text
```
Output:
```bash
Running via Spring preloader in process 26051
      invoke  active_record
      create    db/migrate/20171017210248_create_posts.rb
      create    app/models/post.rb
      invoke    test_unit
      create      test/models/post_test.rb
      create      test/fixtures/posts.yml
      invoke  resource_route
       route    resources :posts
      invoke  scaffold_controller
      create    app/controllers/posts_controller.rb
      invoke    erb
      create      app/views/posts
      create      app/views/posts/index.html.erb
      create      app/views/posts/edit.html.erb
      create      app/views/posts/show.html.erb
      create      app/views/posts/new.html.erb
      create      app/views/posts/_form.html.erb
      invoke    test_unit
      create      test/controllers/posts_controller_test.rb
      invoke    helper
      create      app/helpers/posts_helper.rb
      invoke      test_unit
      invoke    jbuilder
      create      app/views/posts/index.json.jbuilder
      create      app/views/posts/show.json.jbuilder
      create      app/views/posts/_post.json.jbuilder
      invoke  test_unit
      create    test/system/posts_test.rb
      invoke  assets
      invoke    coffee
      create      app/assets/javascripts/posts.coffee
      invoke    scss
      create      app/assets/stylesheets/posts.scss
      invoke  scss
   identical    app/assets/stylesheets/scaffolds.scss
```

Links:
* [model](./app/models/post.rb)
* [migration](./db/migrate/20171017210248_create_posts.rb)
* [route](./config/routes.rb)
* [controller](./app/controllers/posts_controller.rb)
* [views](./app/views/posts/)
