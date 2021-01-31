## App uses Strapi and Next.js. 

Consists of the following:

1. [**frontend**](https://github.com/dariadia/strapped-journals/tree/master/frontend): Next.js application
2. [**backend**](https://github.com/dariadia/strapped-journals/tree/master/backend): Dockerized Strapi application

## Overview

This boilerplate is built using the following technologies:

1. [Chakra UI](https://chakra-ui.com/)
2. [Emotion](https://emotion.sh/)
3. [GraphQL](https://graphql.org/)
4. [Apollo](https://www.apollographql.com/)
5. [NextAuth](https://next-auth.js.org/)
6. [TypeScript](https://www.typescriptlang.org/)

It supports GraphQL Query and Mutation out of the box.

## Prerequisites

1. [Node.js](https://nodejs.org/)
2. [npm](https://www.npmjs.com/)
3. [Docker](https://www.docker.com/)

## Packages

### 1. [**Frontend**](https://github.com/dariadia/strapped-journals/tree/master/frontend): Next.js application

This application is the primary user-facing application. Once it’s up and running (see Development section), it’s available on http://localhost:3000/.

### 2. [**Backend**](https://github.com/dariadia/strapped-journals/tree/master/backend): Dockerized Strapi application

[Strapi](https://strapi.io/) is the leading open-source headless CMS. It’s 100% Javascript, fully customizable and developer-first.

## Installation

### 1. **Clone the application**

```sh
git clone https://github.com/dariadia/strapped-journals.git
```

### 2. **Install necessary dependencies for the frontend application**

```sh
cd frontend && yarn install
```

### 3. **Create a .env file and copy the contents from .env.example (present in frontend directory)**

We might need to run the following command:

```sh
source .env
```

* Get your credentials (e.g. Google client credentials) from your team.

OR

**Create and copy the Google client credentials**

Create a new [Google OAuth Client](https://console.developers.google.com/apis/credentials/oauthclient) and copy the credentials (Client ID and Client Secret) in your .env file.

### 4. **Start the frontend application**

From the frontend directory, we can run the following command to start our Next.js frontend application:

```sh
yarn dev
```

The above command will start the frontend application on [http://localhost:3000/](http://localhost:3000).

### 5. **Go inside the directory of the backend package on another terminal window**

```sh
cd backend
```

### 6. **Start docker-compose**

```sh
docker-compose up
```

We need to start Docker and then run the above command which will change the current directory to the backend package’s directory and then start the backend package. If everything goes well, it’ll be up and running on [http://localhost:1337/graphql](http://localhost:1337/graphql).

## Deployment

TODO 
