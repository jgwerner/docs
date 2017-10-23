`API keys` are used to securely authenticate to your servers, including published RESTful models. Therefore, although the server's URL endpoint is public, authentication to the server can only be done with API Key. All servers, in all public and private projects, are associated to your server's unique API Key.

`API keys` are added as `query parameters` to the URL where the server is located and specified by the `access_token` parameter. For example:

```
access_token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VyX2lkIjoiMjY2NjQ1OWEtMTU2OS00Y2ZiLTg0ZjktMTUxNjJjZjZiOGJkIiwiZW1haWwiOiJ3ZXJuZXIuZ3JlZ0BnbWFpbC5jb20iLCJ1c2VybmFtUSI6Imd3ZXJuZXIiLCJzZXJ2ZXJfaWQiOiJiMWYxZDE4Zi0yMjBkLTQzYjAtYWIwNy1jN2Q3MTUzNThiNzMiLCJpYXQiOjE1MDc5ODcxNjV9.vbtH9CAixqfZGDb46B6JHxiavYicJevs-_SjFCpbAVs
```

!!! note "API Key Standard"
    We have moved our API keys to the open JWT (JSON Web Token) standard.

To share a user server or access a `RESTful endpoint`, simply copy the full URL including the `API Key`. 
