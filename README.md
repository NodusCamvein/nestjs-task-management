# Task Management Application (REST API)

Learned all about NestJS thanks to the following course: https://www.udemy.com/course/nestjs-zero-to-hero/

I installed the NestJS CLI and made use of nest, npm, and yarn commands, although mainly yarn, which made everything smooth. Having a good instructor helped a lot, and I was able to follow and understand the processes required to build a Task Management App, without being too confused at the end...

From the very basics, when we're talking about Modules, Controllers, Providers, and Services, to the creation, reading, updating, and deleting of tasks. The use of DTO's, repositories, statuses, imports, exports, directories, types, uuid's, etc.

Was introduced to NestJS Pipes, and their @Injectable decorator with transform() methods. Global, Handler-level and Parameter-level pipes and their uses. Validation pipes, error handling, and filters.

The use of ORM's, specifically TypeORM, with its pros and cons, and the refactoring of the inital code. Data Mapper vs Active Record, simplification of code and dependency of its strengths. Setting up a connection to a database, and extensive use of entities and repositories, with emphasis on data persistence and restructuring of the previous crud setup.

Commands used:

```bash
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

```
