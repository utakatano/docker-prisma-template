# Prisma Template with Docker/Docker Compose

## Environment

- Node.js ... 16.0.0
- [Prisma](https://www.prisma.io/) ... 2.21.2

## How to run local development

```sh
% docker-compose up -d --build

% docker-compose exec prisma bash

# in the container
/starter $ npm install # if node_modules does not exist
/starter $ npm run dev
```

if the result fails with `npm run dev`, run `npx prisma generate` command and retry it.

__NOTE__
The source code is based on [Prisma official Quickstart page's](https://www.prisma.io/docs/getting-started/quickstart-typescript).
And, the sterter is updated for Apple M1 devices - `@prisma/client@dev` and `@prisma/cli@dev` are installed.

[reference](https://github.com/prisma/prisma/discussions/4739)
