# **Relieve Furniture Platform**

## Table of contents

- [Environments](#environments)
- [Test](#test)
- [Utility](#utility)
- [API](doc/API.md)
- [Frontend](doc/Frontend.md)
- [Services](doc/Services.md)

---

## Environments

### Development Enviroment

Requirements:

- [Docker](https://docs.docker.com/get-docker/)
- [Node.js](https://nodejs.org/en/)
- [npm](https://www.npmjs.com/)

Install :

```bash
npm install
```

Build environment:
(Generate prisma client / create db migration / generate schema.gql)

```bash
npm run build:dev
# then
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

---

### Staging

To build and deploy staging connect to the vercel dashboard.
You'll first need to add a custom domain to your project.
Then setup the  environment variables using Environment Variables UI,
using all the variable in the .env.staging.local.
Check the Preview flag and select the staging git branch

<img src="https://www.datocms-assets.com/31049/1619043001-add-preview-var.png?auto=format&fm=webp&w=948" alt="drawing" width="500px"/>



https://relieve-furniture-platform-staging.vercel.app/

---

### Production

https://relieve-furniture-platform.vercel.app/

---

## Test

We use [Cypress](https://www.cypress.io/) as testing tool

- CLI

```bash
npm run test:<FOLDERNAME>
# e.g.
npm run test:api
# or
npm run test:graphql
```

- Component

```bash
npm run test:component
```

- GUI

```shell
npm run cypress:open
```

## Utility

### Seed

```bash
npm run db:seed:<env>
 # e.g.
npm run db:seed:dev
# or
npm run db:seed:staging
```

### Reset

```bash
npm run db:reset:<env>
 # e.g.
npm run db:reset:dev
# or
npm run db:reset:staging
```

### Prisma Studio

```bash
npm run prisma:studio:<env>
 # e.g.
npm run prisma:studio:dev
# or
npm run db:prisma:staging
# or
npm run db:prisma:production

```
