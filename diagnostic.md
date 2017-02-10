# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.

What is the purpose of a backend?

```md
to organize the data/processes needed for the web application to communicate between the server and client
```

Which layer in the MVC pattern is used by the controller to fetch data?

```md
Model
```

Which layer in the MVC pattern communicates with the model?

```md
Controller
```

Why don't we use views in our interpretation of the MVC pattern?

```md
Serializers replace all the views we care about
```

What does C.R.U.D stand for?

```md
CREATE
READ
UPDATE
DESTROY
```

In which part of the MVC pattern can we find C.R.U.D actions?

```md
Controller
```

List at least 5 standard rails actions that C.R.U.D requests correspond to?

```md
.exists?
.create!
.find_by
.new
.save
.where
.last
```

A user action fires a `GET` request for `/people/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list)

```md
The user sents the request (URL/verb)
The router receives the request and sends to the controller
The controller sends the request to the model
The model communicates with the database to find the data associated `/people/1`
The model sends the object to the controller
The controller sends the response to the user
```

What is the command to generate a new rails-api app?

```bash
rails new my_api --api
```

What is the command to start an instance of a rails server?

```bash
bin/rails server
```

What are the commands to drop, create, migrate and seed a database from the command
line? (5 bullet points)

```bash
bin/rake db:drop
bin/rake db:create
bin/rake db:migrate
bin/rake db:seed
```

What is the command to scaffold a pet with a name and age attributes (hint:
Also think of the data types for each attribute)?

```bash
bin/rails generate scaffold pet name:string age:integer
```
