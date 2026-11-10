# Datacircle: best GTM API

Find the best GTM APIs. We benchmark all the GTM APIs and we put the results on our website: https://datacircle.dev

This action asks the open Datacircle API (https://api.datacircle.dev/v1, no key) for the best plans of a GTM API.

```yaml
- uses: waynehamadi/datacircle-api-action@v1
  id: best
  with:
    api: email-finder
- run: echo '${{ steps.best.outputs.result }}'
```

Leave `api` empty to list every API. The spec is at https://api.datacircle.dev/v1/openapi.json.
