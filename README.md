# Install ubuntu packages from proper mirror

Example:

```yaml
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: stbuehler/action-apt@v1
        with:
          cache-key: apt-${{ runner.os }}-${{ github.run_id }}
          packages: libsome-build-dependency-dev
      ...
```
