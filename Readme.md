
## Background

In order to become a better full stack developer it is necessary to have an in-depth understanding of the main technologies used by Trio in the current project. Those are: typescript, typeorm, Node with express, and MySql for the DB. And a good understanding of Docker is also recommended.

## Requirements

It should use:
- NodeJS
- Express
- TypeORM
- MySQL
- CRUD for users

It should implement:
- Database Normalization
- Clean code / architecture

## Objectives

Create a simple application, a proof-of-concept for a Backend App, using the same set of technologies used in the Trio Zion project.

### Other Project Ideas:

- BLOG API backend application
- Book club App
	- where you and your friends can share your favorite books and discuss them (like Goodreads). 
	- The backend could be a simple Node CRUD app
	- Front end could be a single page Vue app and play with Vue router and Vuex.
- Build an API for The Dark Tower (or the Honor Harrington book series) characters


# Technical Design

1. Create a Docker container for a new MySql DB
2. Install dependencies
	- Express
	- Typescript
	- TypeORM

3. Create a simple NodeJS server with 4 endpoints
	- api/user/create => POST
	- api/user/:id/update => UPDATE
	- api/user/:id/delete => DELETE
	- api/user/:id => GET

4. Migration
	- CreateUserTable
		- Id: uuid
		- userName: string
		- createdAt: Date

5. Model
	- User

6. Type
	- User

7. Repository
	- UserRepositoryTypeORM

8. Use-cases
	- Create-user
	- Update-user
	- Delete-user
	- Get-user

9. Tests
It should create a new user
It should throw an error if the user already exists
It should update an existing user
It should throw an error if a user doesn’t exist
It should delete a user
It should throw an error if the user to be deleted doesn’t exist
It should get a user
It should throw an error if the user doesn’t exist
Schemas
Create-user
get-user
Update-user
delete-user
Seed
userSeed
