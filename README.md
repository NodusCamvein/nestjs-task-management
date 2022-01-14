# Task Management Application (REST API)

Learned all about NestJS thanks to the following course: https://www.udemy.com/course/nestjs-zero-to-hero/

I installed the NestJS CLI and made use of nest, npm, and yarn commands, although mainly yarn, which made everything smooth. Having a good instructor helped a lot, and I was able to follow and understand the processes required to build a Task Management App, without being too confused at the end...

From the very basics, when we're talking about Modules, Controllers, Providers, and Services, to the creation, reading, updating, and deleting of tasks. The use of DTO's, repositories, statuses, imports, exports, directories, types, uuid's, etc.

Was introduced to NestJS Pipes, and their @Injectable decorator with transform() methods. Global, Handler-level and Parameter-level pipes and their uses. Validation pipes, error handling, and filters.

The use of ORM's, specifically TypeORM, with its pros and cons, and the refactoring of the inital code. Data Mapper vs Active Record, simplification of code and dependency of its strengths. Setting up a connection to a database, and extensive use of columns, entities and repositories, with emphasis on data persistence and restructuring of the previous crud setup.

Went through a good amount of authentication and authorization content, the use of Postman, Docker, PostgreSQL, and pgAdmin for task simulations and observations.

Learned about JWT, its structure, and every detail regarding authentication and authorization. From "strong" passwords, bearer tokens, hashing, salts, bcrypt, to signups and signins, requests and validations, and got a decent grasp on error handling, while being able to identify them with console logs.

Further emphasis on tasks and users, with database relation. Introduction to OneToMany and ManyToOne, have users create their own tasks and implemented nestjs logger.

I was surprised that configurations were a "thing", it improved the app, and I implemented the NestJS Config module, where TypeORM, Schema Validation, and JWT secrets were put in use, and the same could be said regarding environment variables, and did more error handling and spotting/logging.

Made use of the front-end application provided by the course, and enabled Cors: https://github.com/arielweinberger/task-management-frontend

Installed and deployed NestJS app to Heroku, making use of the provided database credentials, and ssl for security.

It was challenging to memorize, and I learned a bunch of things that I'll have to try to remember when needed. All in all, this was fun.

Commands used:

```
yarn global add @nestjs/cli
nest -v
nest new nestjs-task-management (chose yarn over npm in this case)
nest g
nest g --help
nest g module tasks
yarn start:dev
nest g controller tasks --no-spec
nest g service tasks --no-spec
yarn add uuid
yarn add class-validator class-transformer
docker
docker run --name postgres-nest -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres
docker container ls
docker container stop 'name of container or ID without quotes'
docker container start 'name of container or ID without quotes'
docker container rm 'name of container or ID without quotes'
yarn add typeorm @nestjs/typeorm pg
yarn remove uuid (good practice to remove packages that you don't use anymore)
nest g module auth
nest g service auth --no-spec
nest g controller auth --no-spec
yarn add bcrypt
yarn add @nestjs/jwt @nestjs/passport passport passport-jwt
yarn add @types/passport-jwt
yarn global add cross-env
"start:dev": "cross-env STAGE=dev nest start --watch",
yarn add @nestjs/config
replaced "start:dev": "cross-env STAGE=dev nest start --watch,  (same with debug, prod, and test)
yarn add @hapi/joi
yarn add -D @types/hapi__joi
yarn global add heroku
heroku -v
heroku login
heroku addons:create heroku-postgresql:hobby-dev -a 'name of the app without quotes'
heroku git:remote -a 'name of the app without quotes'
heroku config:set NPM_CONFIG_PRODUCTION=false
heroku config:set NODE_ENV=production
heroku config:set STAGE=prod
 heroku config:set DB_HOST=
 heroku config:set DB_PORT=
 heroku config:set DB_USERNAME=
 heroku config:set DB_PASSWORD=
 heroku config:set DB_DATABASE=
 heroku config:set DB_DATABASE=
 heroku config:set JWT_SECRET=
 git add .
 git commit -m "Going live"
 git push -f heroku HEAD:master
 heroku logs --tail
```

Front-end Commands:

```
yarn
yarn upgrade
yarn start
```
