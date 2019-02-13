# x-replaced-by

Enhances the deprecated property by providing the path and verb that should be used instead.

```yaml
paths:
  /v1/user:
    post:
      ...
      deprecated: true
      x-replaced-by:
        path: '/v2/user'
        verb: post
  /v2/user:
    post:
      ...
```
