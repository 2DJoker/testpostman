# Postman CRUD setup (from scratch)

## Files
- `CRUD_Books_Collection.postman_collection.json`
- `CRUD_Books_Environment.postman_environment.json`

## How to run in Postman
1. Open Postman.
2. Import both JSON files from the `postman` folder.
3. Select environment **CRUD Books Env**.
4. Open collection **CRUD Books Tests**.
5. Run collection in Collection Runner (all 5 requests).

## What is implemented
- 5 requests:
  - GET list by `userId`
  - POST create (with Pre-request Script for random `bookTitle`)
  - GET by `postId`
  - PUT by `postId`
  - DELETE by `postId`
- Collection variable: `baseUrl`.
- Environment variable: `userId` (plus reused `postId`, `bookTitle`, `createdId`).
- In each request tests include response time check.
- Each request has at least 2 assertions.

## API used
`https://jsonplaceholder.typicode.com`
