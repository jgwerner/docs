`API keys` are required to securely access your servers, including published RESTful models endpoints. While all servers have a publicly-addressable URL, authentication to the server can only be done with each server's unique API key.

`API keys` are added as a query parameter to the server's URL and are specified using the access_token key. For example::

```
access_token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ1c2VyX2lkIjoiMjY2NjQ1OWEtMTU2OS00Y2ZiLTg0ZjktMTUxNjJjZjZiOGJkIiwiZW1haWwiOiJ3ZXJuZXIuZ3JlZ0BnbWFpbC5jb20iLCJ1c2VybmFtUSI6Imd3ZXJuZXIiLCJzZXJ2ZXJfaWQiOiJiMWYxZDE4Zi0yMjBkLTQzYjAtYWIwNy1jN2Q3MTUzNThiNzMiLCJpYXQiOjE1MDc5ODcxNjV9.vbtH9CAixqfZGDb46B6JHxiavYicJevs-_SjFCpbAVs
```

!!! note "API Key Standard"
    Our API keys adhere to the JWT (JSON Web Token) standard.

To share a user server or access a `RESTful endpoint`, simply copy the full URL including the `API key`.
