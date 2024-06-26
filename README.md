Note: Forked this repo to play around with GraphQL concepts via .NET & Hot Chocolate

# (Odyssey Course) Federation with .NET (C#) & Hot Chocolate 

Welcome to the starter code for **Federation with .NET (C#) & Hot Chocolate**. You can find the [course lessons and instructions](https://apollographql.com/tutorials/federation-hotchocolate) on Odyssey, [Apollo](https://apollographql.com)'s learning platform.

## How to use this repo

The course will walk you step by step on what to do. This codebase is the starting point of your journey!

This project uses [.NET CLI](https://learn.microsoft.com/en-us/dotnet/core/tools/) and requires .NET 7.0+ runtime. In order to build the project locally, run:

```shell
dotnet build
```

To start the server, from the root directory, run:

```shell script
dotnet watch
```

Right now, the project is a GraphQL server returning playlist and track data at `http://localhost:5059/graphql`. You can use [Apollo Sandbox](https://studio.apollographql.com/sandbox?endpoint=http://localhost:5059/graphql) to connect to the endpoint and send queries.

Try running this query:

```graphql
query GetFeaturedPlaylists {
  featuredPlaylists {
    id
    name
    description
    tracks {
      id
      name
      explicit
      uri
    }
  }
}
```

The `final` branch of this repo contains the final stage of the course, with all of the steps and code completed! If you get stuck, you can refer to it and compare your code.

## Getting Help

This repo is _not regularly monitored_.

For any issues or problems concerning the course content, please refer to the [Odyssey topic in our community forums](https://community.apollographql.com/tags/c/help/6/odyssey). You can also [join the Apollo Discord](https://discord.gg/graphos).
