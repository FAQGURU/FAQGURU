## GraphQL

[What is GraphQL?](#what-is-graphql)

[Is GraphQL a Database Technology?](#is-graphql-a-database-technology)

[Is GraphQL only for React / Javascript Developers?](#is-graphql-only-for-react--javascript-developers)

[How to do Error Handling?](#how-to-do-error-handling)

[Where is GraphQL useful?](#where-is-graphql-useful)

[What is GraphQL schema?](#what-is-graphql-schema)

[How to do Authentication and Authorization?](#how-to-do-authentication-and-authorization)

[Does GraphQL Support Offline Usage?](#does-graphql-support-offline-usage)

[How to do Server-side Caching?](#how-to-do-server-side-caching)

[List the key concepts of the GraphQL query language](#list-the-key-concepts-of-the-graphql-query-language)

[Explain the main difference between REST and GraphQL](#explain-the-main-difference-between-rest-and-graphql)

[What kind of operations could GraphQL schema have?](#what-kind-of-operations-could-graphql-schema-have)

[Are there any disadvantages to GraphQL?](#are-there-any-disadvantages-to-graphql)



### What is GraphQL?

GraphQL is a query language created by [Facebook](http://facebook.github.io/) in 2012 which provides a **common interface between the client and the server for data fetching and manipulations**.

The client asks for various data from the GraphQL server via queries. The response format is described in the query and defined by the client instead of the server: they are called **client‐specified queries**.  
The structure of the data is not hardcoded as in traditional REST APIs - this makes retrieving data from the server more efficient for the client.

###### Source

* https://www.howtographql.com/advanced/5-common-questions/

[[↑] Back to top](#GraphQL)
### Is GraphQL a Database Technology?

No. GraphQL is often confused with being a database technology. This is a misconception, GraphQL is a _query language_ for APIs - not databases. In that sense it’s database agnostic and can be used with any kind of database or even no database at all.

###### Source

* https://www.howtographql.com/advanced/5-common-questions/

[[↑] Back to top](#GraphQL)
### Is GraphQL only for React / Javascript Developers?

No. GraphQL is an API technology so it can be used in any context where an API is required.

On the _backend_, a GraphQL server can be implemented in any programming language that can be used to build a web server. Next to Javascript, there are popular reference implementations for Ruby, Python, Scala, Java, Clojure, Go and .NET.

Since a GraphQL API is usually operated over HTTP, any client that can speak HTTP is able to query data from a GraphQL server.

*Note*: GraphQL is actually transport layer agnostic, so you could choose other protocols than HTTP to implement your server.

###### Source

* https://www.howtographql.com/advanced/5-common-questions/

[[↑] Back to top](#GraphQL)
### How to do Error Handling?

A successful GraphQL query is supposed to return a JSON object with a root field called `"data"`. If the request fails or partially fails (e.g. because the user requesting the data doesn’t have the right access permissions), a second root field called `"errors"` is added to the response:
```js
    {
      "data": { ... },
      "errors": [ ... ]
    }
```   

###### Source

* https://www.howtographql.com/advanced/5-common-questions/

[[↑] Back to top](#GraphQL)
### Where is GraphQL useful?

GraphQL helps where your **client needs a flexible response** format to avoid extra queries and/or massive data transformation with the overhead of keeping them in sync.

Using a GraphQL server makes it very easy for a client side developer to change the response format without any change on the backend.

With GraphQL, you can describe the required data in a more natural way. It can speed up development, because in application structures like **top-down rendering** in React, the required data is more similar to your component structure.

###### Source

* https://blog.risingstack.com/graphql-overview-getting-started-with-graphql-and-nodejs/

[[↑] Back to top](#GraphQL)
### What is GraphQL schema?

Every GraphQL server has two core parts that determine how it works: a schema and resolve functions.

The *schema* is a model of the data that can be fetched through the GraphQL server. It defines what queries clients are allowed to make, what types of data can be fetched from the server, and what the relationships between these types are. 

Consider:

```css
type Author {
  id: Int
  name: String
  posts: [Post]
}
type Post {
  id: Int
  title: String
  text: String
  author: Author
}
type Query {
  getAuthor(id: Int): Author
  getPostsByTitle(titleContains: String): [Post]
}
schema {
  query: Query
}
```

###### Source

* https://dev-blog.apollodata.com/graphql-explained-5844742f195e?_ga=2.144563709.979734643.1528637959-111420911.1528637959

[[↑] Back to top](#GraphQL)
### How to do Authentication and Authorization?

Authentication and authorization are often confused. _Authentication_ describes the process of claiming an _identity_. That’s what you do when you log in to a service with a username and password, you authenticate yourself. _Authorization_ on the other hand describes _permission rules_ that specify the access rights of individual users and user groups to certain parts of the system.

Authentication in GraphQL can be implemented with common patterns such as [OAuth](https://oauth.net/).

To implement authorization, it is [recommended](http://graphql.org/learn/authorization/) to delegate any data access logic to the business logic layer and not handle it directly in the GraphQL implementation.

###### Source

* https://www.howtographql.com/advanced/5-common-questions/

[[↑] Back to top](#GraphQL)
### Does GraphQL Support Offline Usage?

GraphQL is a query language for (web) APIs, and in that sense by definition only works online. However, offline support on the client-side is a valid concern. The caching abilities of Relay and Apollo might already be enough for some use cases, but there isn’t a popular solution for actually persisting stored data yet.

###### Source

* https://www.howtographql.com/advanced/5-common-questions/

[[↑] Back to top](#GraphQL)
### How to do Server-side Caching?

One common concern with GraphQL, especially when comparing it to REST, are the difficulties to maintain server-side cache. With REST, it’s easy to cache the data for each endpoint, since it’s sure that the _structure_ of the data will not change.

With GraphQL on the other hand, it’s not clear what a client will request next, so putting a caching layer right behind the API doesn’t make a lot of sense.

Server-side caching still is a challenge with GraphQL.

###### Source

* https://www.howtographql.com/advanced/5-common-questions/

[[↑] Back to top](#GraphQL)
### List the key concepts of the GraphQL query language

**Key concepts of the GraphQL** query language are:

*   Hierarchical
*   Product‐centric
*   Strong‐typing
*   Client‐specified queries
*   Introspective

###### Source

* https://blog.risingstack.com/graphql-overview-getting-started-with-graphql-and-nodejs/

[[↑] Back to top](#GraphQL)
### Explain the main difference between REST and GraphQL

The main and most important difference between REST and GraphQL is that *GraphQL is not dealing with dedicated resources, instead everything is regarded as a graph and therefore is connected and can be queried to app exact needs*.

###### Source

* https://medium.com/codingthesmartway-com-blog/rest-vs-graphql-418eac2e3083

[[↑] Back to top](#GraphQL)
### What kind of operations could GraphQL schema have?

There are three kinds of operation available at the entry points to the schema:

* Schema must have `query` object type whose fields are the set of query endpoints of the server application.
* A schema may optionally have `mutation` object type, whose fields are the set of mutations available on the server.
* The schema may have a `subscription` object type, whose fields are the set of subscriptions.

###### Source

* https://medium.com/coffee-and-codes/a-beginners-dive-into-graphql-part-2-86df02361736

[[↑] Back to top](#GraphQL)
### Are there any disadvantages to GraphQL?

Disadvantages:

*   You **need to learn** how to set up GraphQL. The ecosystem is still rapidly evolving so you have to keep up.
*   You need to send the queries from the client, you can just send strings but if you want more comfort and caching you'll use a client library -> **extra code** in your client
*   You need to define the schema beforehand => **extra work** before you get results
*   You need to have a graphql endpoint on your server => **new libraries** that you don't know yet
*   Graphql queries are **more bytes** than simply going to a REST endpoint
*   The server needs to do **more processing** to parse the query and verify the parameters

###### Source

* https://stackoverflow.com/questions/40689858/are-there-any-disadvantages-to-graphql

[[↑] Back to top](#GraphQL)
