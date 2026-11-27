---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formulasignal-com-category-api-openapi.yml
  format: yaml
  label: FormulaSignal Category API
  slug: formulasignal-com-category-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-category-api-openapi.yml
- filename: formulasignal-com-context-api-openapi.yml
  format: yaml
  label: FormulaSignal Context API
  slug: formulasignal-com-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-context-api-openapi.yml
- filename: formulasignal-com-ledger-api-openapi.yml
  format: yaml
  label: FormulaSignal Ledger API
  slug: formulasignal-com-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-ledger-api-openapi.yml
- filename: formulasignal-com-meta-api-openapi.yml
  format: yaml
  label: FormulaSignal Meta API
  slug: formulasignal-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-meta-api-openapi.yml
- filename: formulasignal-com-products-api-openapi.yml
  format: yaml
  label: FormulaSignal Products API
  slug: formulasignal-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-products-api-openapi.yml
- filename: formulasignal-com-record-api-openapi.yml
  format: yaml
  label: FormulaSignal Record API
  slug: formulasignal-com-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-record-api-openapi.yml
- filename: formulasignal-com-signals-api-openapi.yml
  format: yaml
  label: FormulaSignal Signals API
  slug: formulasignal-com-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-signals-api-openapi.yml
- filename: formulasignal-com-watch-api-openapi.yml
  format: yaml
  label: FormulaSignal Watch API
  slug: formulasignal-com-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formulasignal-com/openapi/formulasignal-com-watch-api-openapi.yml
auth_types: []
description: FormulaSignal authenticates using an API key sent as a bearer token in the Authorization header, with an alternative plain header X-FormulaSignal-Key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FormulaSignal Authentication
name_suffix: Authentication
oauth_flows: []
overview: FormulaSignal declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FormulaSignal
provider_slug: formulasignal-com
scheme_count: 2
schemes:
- evidence: 'curl -s https://formulasignal.com/api/v1/products/resolve \ -H "Authorization: Bearer $FORMULASIGNAL_API_KEY" \ -H "Content-Type: application/json" \ -d ''{"identifier":"C4 Original"}'''
  header: Authorization
  how_to_obtain: Get a free API key via the developer portal; the key is shown once after you provide an email address and follow the sign‑in link.
  location: header
  name: FormulaSignal API Key
  type: http-bearer
- evidence: If your client rejects Authorization , send the key as X-FormulaSignal-Key with no Bearer prefix.
  header: X-FormulaSignal-Key
  how_to_obtain: Get a free API key via the developer portal; the key is shown once after you provide an email address and follow the sign‑in link.
  location: header
  name: FormulaSignal API Key (alternative header)
  type: apiKey
slug: formulasignal-com-authentication
source_filename: formulasignal-com-authentication.yml
source_heading: Authentication Profile
source_url: https://formulasignal.com/developers/keys
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://formulasignal.com/developers/keys\nsources:\n- https://formulasignal.com/developers/keys\n- https://formulasignal.com/developers\n- https://formulasignal.com/developers/mcp\ndescription: FormulaSignal authenticates using an API key sent as a bearer token in the Authorization header, with an alternative plain header\n  X-FormulaSignal-Key.\nschemes:\n- type: http-bearer\n  name: FormulaSignal API Key\n  evidence: 'curl -s https://formulasignal.com/api/v1/products/resolve \\ -H \"Authorization: Bearer $FORMULASIGNAL_API_KEY\" \\ -H \"Content-Type:\n    application/json\" \\ -d ''{\"identifier\":\"C4 Original\"}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Get a free API key via the developer portal; the key is shown once after you provide an email address and follow the sign‑in\n    link.\n- type: apiKey\n  name: FormulaSignal API Key (alternative header)\n\
  \  evidence: If your client rejects Authorization , send the key as X-FormulaSignal-Key with no Bearer prefix.\n  location: header\n  header: X-FormulaSignal-Key\n  how_to_obtain: Get a free API key via the developer portal; the key is shown once after you provide an email address and follow the sign‑in\n    link.\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other authentication methods are documented.\ndocs: https://formulasignal.com/developers/keys\n"
source_yaml_url: https://artifacts.apis.io/formulasignal-com/authentication/formulasignal-com-authentication.yml
summary_line: 2 schemes
tags:
- Health
- Supplements
- Monitoring
- Consumer App
- Nutrition
---
