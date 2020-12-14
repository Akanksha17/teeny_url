# Backend for shortening URLs.

## Graphql APIs developed using django-graphene.

1. Available url query grahql schema:

```
query {
  urls {
    id
    fullUrl
    urlHash
    clicks
    createdAt
  }
}
```

2. Available Mutation to shorten the url:

```
mutation {
  createUrl(fullUrl:"<url to be shortened>") {
    url {
      id
      fullUrl
      urlHash
      clicks
      createdAt
    }
  }
}
```

Grahql interface can be accessed at:
http://localhost:8000/graphql/
