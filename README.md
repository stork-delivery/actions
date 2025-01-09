# Stork Create Version Action

This action creates a new version of an app in the Stork Platform.

```yaml
jobs:
  create_version:
    name: Create Stork Version
    runs-on: ubuntu-latest

    steps:
      - uses: stork-delivery/create_version@main
        with:
          version: ${{ github.ref_name }}
          app-id: ${{ secrets.STORK_APP_ID }}
          api-key: ${{ secrets.STORK_API_KEY }}
```
