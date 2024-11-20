# actions.envsubst

Substitutes the values of environment variables using envsubst.

**This result will override origin files**

```yaml
name: Example

on: push

jobs:
  example:
    name: Example
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: buka-inc/actions.envsubst@v1
        with:
          files: ./templates/**/*.json
        env:
          VALUE: "Hello World"
```
