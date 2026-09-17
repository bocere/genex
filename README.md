# genex

Generate REST API reference documentation from
an OpenAPI spec and a companion set of request/response
examples.

Given `openapi.yaml` (the API contract) and `examples.yaml` (curl commands,
summaries, and sample request/response bodies for each operation), `genex`
generates one DITA concept topic per endpoint/method, ready to be built into
an API reference guide. 

Run it from this directory:

```bash
python3 genex
```

## Requirements

- Python 3 with `pyyaml`, `lxml`, and `requests`

## Notes

`examples.yaml` and `openapi.yaml` currently document a small, generic
example commerce API (orders, customers, products, settings) rather than
any specific product's real API — useful as a template for wiring up a
new doc set with this tool.
