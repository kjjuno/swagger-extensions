# x-remove-on

Enhances the deprecated property by providing the date that an endpoint is schedules for removal.

```yaml
paths:
  /v1/user:
    post:
      ...
      deprecated: true
      x-remove-on: 1/12/2020
```
