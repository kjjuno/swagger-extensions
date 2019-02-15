# x-replaced-by

Enhances the deprecated property by providing the path and verb that should be used instead.

```yaml
paths:
  /v1/user:
    post:
      ...
      deprecated: true
      x-replaced-by:
        - description: some description asdlfkj
          path: '/v2/user'
          verb: post
        - description: some description asdlfkj
          path: '/v2/user'
          verb: post
    get:
       ...
      x-replaced-by:
        description: some description asdlfkj
          path: '/v2/user'
          verb: post
  /v2/user:
    post:
      ...
```
