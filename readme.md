# decoupled-pern-jwt-auth-template-back-end 

## Model Express App

This repository has an express app at many different states to model the setup for different situations. Explore the branches and checkout this readme to learn about each state.

## express-ejs-nodb Branch

This branch shows an express app that deliver a JSON API with CRUD functionality using a Postgres Database with the Sequelize ORM.

This API implement multi-user JWT token authentication.

Keep in mind you'll need to run migration, documentation can be found here on how:

https://sequelize.org/docs/v6/other-topics/migrations/#running-migrations

The models/migration folders reflect setting up models using the sequelize CLI, the models_ folder represents writing out a database connection and models manually which requires to pre-make tables.

|Route|Method|Path|Response|
|-----|------|----|--------|
|Index|GET|/todo| returns all todos as json |
|Show|GET|/todo/:id| returns a single todo as json |
|Create|POST|/todo| receives json body, creates new todo, returns updated list of todos |
|Update|PUT|/todo/:id| receives json body, updates todo, returns updated list as json |
|Destroy|Delete|/todo/:id| Deletes a todo and returns updated list as json |

checkout comments for more details

Any variables like `process.env.PORT` are assumed to have been defined in a .env file like so...

```
PORT=4000
```