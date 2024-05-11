# Notes About Federation with .NET & Hot Chocolate
** tutorial link: https://www.apollographql.com/tutorials/federation-hotchocolate

## supergraph: federated graphql architecture
Creates a network of
* company data
* microservices
* digital capabilities
* easier composition and validation from backend
* one-stop shop for frontend wihtout having to write tedious boilerplate code


## introducing federation
As API grows, it becomes harder to manage, scale and deploy.
* divide APIs capabilities across multiple GraphQL powered microservices
* each of these microservices are called subgraph
* they form the foundation of our subgraph
* introduce router to divide queries to appropriate subgraphs
* nothing changes for the clients, they still communicate directly with a single GraphQL endpoint