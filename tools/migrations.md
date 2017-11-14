### Django
```py
# edit / create [app]/models.py
class Post(models.Model):
    title = models.CharField(max_length=250)
    content = models.TextField()
```
```bash
$ python manage.py makemigrations
    Migrations for 'posts':
      posts/migrations/0001_initial.py
        - Create model Post
$ python manage.py migrate
    Operations to perform:
      Apply all migrations: posts
    Running migrations:
      Applying posts.0001_initial... OK
```
Migrations are numbered, and must be run in the correct order. If two migrations are created at the same time on the same app concurrently, they will conflict regardless of the changes they make.
[Example Model File](../examples/django_startapp/posts/models.py)
[Example Migration File](../examples/django_startapp/posts/migrations/0001_initial.py)

### Rails
```bash
$ rails generate model Post title:string content:text
    db/migrate/20171017210248_create_posts.rb
    app/models/post.rb
```
[Example Model File](../examples/rails_scaffolding/app/models/post.rb)
[Example Migration File](../examples/rails_scaffolding/db/migrations/20171017210248_create_posts.rb)
