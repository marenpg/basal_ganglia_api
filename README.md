# Murine Basal Ganglia Web Solution - GraphQL API
This repository is a part of the master's thesis *"Graph-based representation, integration, and analysis of neuroscience data &mdash; The case of the murine basal ganglia"*.
In this thesis, we investigate aspects of graph-based data representation in the neuroscience domain. 
The data set basis is a relational database published by Bjerke et al. (2019) of quantitative neuroanatomical data about the healthy rat and mouse basal ganglia ([DOI:10.25493/DYXZ-76U](https://doi.org/10.25493/DYXZ-76U)).

The API is based on the [GRANDstack Starter - GraphQL API](https://github.com/grand-stack/grand-stack-starter). For more information on the GRANDStack, visit https://grandstack.io/. This directory contains a GraphQL API of the murine basal ganglia graph database. The application connects with a Neo4j database instance.

The API solution is deployed through [Heroku](https://www.heroku.com/) and is available at https://basal-ganglia-graphql.herokuapp.com/graphql.

## Quick Start

Install dependencies:

```
npm install
```

Start the GraphQL service in development mode:

```
npm run start-dev
```

This will start the GraphQL service (by default on localhost:4000) where you can issue GraphQL requests or access GraphQL Playground in the browser:

## Configure

Configuration is done with environment variables specified in `.env`.
The application needs the following variables: The Neo4j database password: `NEO4J_PASSWORD`, The Neo4j database bolt URL: `NEO4J_URI`, and The Neo4j database username: `NEO4J_USER`.
