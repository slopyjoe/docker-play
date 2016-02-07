== Docker Play source code

The source code for `Rails with Docker`. This serves as the baseline Rails application with nothing dockerized yet.

##Setting up the database
~~~
psql
> create role dockerplay with createdb login password 'password1';
~~~
Run migrations
~~~
rake db:create
rake db:migrate
rake db:seed
~~~

Run `rails server` and navigate to `localhost:3000/items`.
