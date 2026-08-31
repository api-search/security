---
api_key_in:
- header
api_specs:
- filename: opensanctions-api-openapi.yml
  format: yaml
  label: OpenSanctions Screening API
  slug: opensanctions-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opensanctions/refs/heads/main/openapi/opensanctions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Opensanctions Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenSanctions secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenSanctions
provider_slug: opensanctions
scheme_count: 1
schemes:
- example_header: 'Authorization: ApiKey xxxxxxxxxxxxxxxxxxxxxxxx'
  in: header
  name: ApiKeyAuth
  note: 'A custom scheme, not RFC 6750 Bearer: the Authorization header carries the literal prefix `ApiKey`, not `Bearer`. The yente-mcp MCP server is the one exception — it accepts `Authorization: Bearer <key>` from the MCP client and translates it before forwarding.'
  parameter_name: Authorization
  sources:
  - https://www.opensanctions.org/docs/api/authentication/
  type: apiKey
  value_format: ApiKey <key>
slug: opensanctions-authentication
source_filename: opensanctions-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: openapi/opensanctions-api-openapi.yml\ndocs: https://www.opensanctions.org/docs/api/authentication/\nnote: >-\n  DERIVE returned nothing: the published OpenAPI declares an EMPTY\n  components.securitySchemes and no top-level `security` requirement, even though\n  every data endpoint requires a key. This profile is therefore SEARCHED from the\n  provider's own authentication docs and confirmed by a live unauthenticated probe.\n  The missing securityScheme is the single largest contract-quality gap in this\n  provider's spec and is captured as a recommendation in\n  overlays/opensanctions-api-overlay.yaml.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  spec_declared: false\n  docs_declared: true\nschemes:\n  - name: ApiKeyAuth\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    value_format: \"ApiKey <key>\"\n    example_header: \"Authorization: ApiKey xxxxxxxxxxxxxxxxxxxxxxxx\"\
  \n    sources: [https://www.opensanctions.org/docs/api/authentication/]\n    note: >-\n      A custom scheme, not RFC 6750 Bearer: the Authorization header carries the\n      literal prefix `ApiKey`, not `Bearer`. The yente-mcp MCP server is the one\n      exception — it accepts `Authorization: Bearer <key>` from the MCP client and\n      translates it before forwarding.\nkey_management:\n  issue_url: https://www.opensanctions.org/api/\n  account_url: https://www.opensanctions.org/account/\n  env_var: OPENSANCTIONS_API_KEY\n  trial: 30-day complimentary trial on registration with a business email address\n  free_keys: >-\n    Free keys are offered for public-interest work — journalism, civil society and\n    academia — by contacting support.\n  rotation_policy: not documented\nunauthenticated_surface:\n  - operation: healthz_healthz_get\n    path: /healthz\n    probed_status: 200\n  - operation: catalog_catalog_get\n    path: /catalog\n    probed_status: 200\n  - operation: readyz_readyz_get\n\
  \    path: /readyz\n    probed_status: not-probed\nself_hosted:\n  product: yente\n  docs: https://www.opensanctions.org/docs/on-premise/\n  note: >-\n    A self-hosted yente instance needs no API key at all (the SDK's `base_url=`\n    kwarg targets it with `api_key` unset). POST /updatez is the one write\n    operation and is guarded separately, returning 403 \"Authorization error.\"\nx-evidence:\n  fetched: '2026-08-27'\n  probes:\n    - url: https://www.opensanctions.org/docs/api/authentication/\n      status: 200\n    - url: https://api.opensanctions.org/search/default?q=test\n      status: 401\n      body: '{\"detail\":\"No API key provided.\"}'\n    - url: https://api.opensanctions.org/healthz\n      status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensanctions/refs/heads/main/authentication/opensanctions-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Sanctions Screening
- Anti-Money Laundering
- Politically Exposed Persons
- Compliance
- Financial Crime
- Know Your Customer
- Entity Resolution
- Open Data
- Risk Data
- Due Diligence
- Public APIs
- agent-native
---
