# x-replaced-by

Enhances the deprecated property by providing the path and verb that should be used instead.

```yaml
paths:
  /v1/user:
    post:
      ...
      deprecated: true
      x-replaced-by:
        - description: Handles only the creation of users
          path: '/v2/user'
          verb: post
        - description: Handles the update of a user
          path: '/v2/user/{id}'
          verb: put
    get:
       ...
      x-replaced-by:
        description: Retrieves the user object
        path: '/v2/user'
        verb: post
  /v2/user:
    post:
      ...
  /v2/user/{id}:
    put:
      ...
```
