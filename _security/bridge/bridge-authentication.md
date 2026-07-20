---
api_key_in:
- header
api_specs:
- filename: bridge-openapi-original.json
  format: json
  label: Bridge API
  slug: bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge/refs/heads/main/openapi/bridge-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Bridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bridge secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bridge
provider_slug: bridge
scheme_count: 1
schemes:
- in: header
  name: ApiKey
  parameter: Api-Key
  sources:
  - openapi/bridge-openapi-original.json
  type: apiKey
slug: bridge-authentication
source_filename: bridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/bridge-openapi-original.json\ndocs: https://apidocs.bridge.xyz/api-reference/api-keys/create-a-scoped-api-key\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  sources:\n  - openapi/bridge-openapi-original.json\nscoped_keys:\n  supported: true\n  scopes_artifact: scopes/bridge-scopes.yml\n  scope_count: 68\n  max_scoped_keys_per_developer: 500\n  subsetting: Callers may only grant scopes they themselves hold; scoped keys need the api_key:create scope to mint further keys.\nenvironments:\n- name: production\n  base_url: https://api.bridge.xyz/v0\n  key_prefix: null\n- name: sandbox\n  base_url: https://api.sandbox.bridge.xyz/v0\n  key_prefix: sk-test\nnotes: >\n  Every request authenticates with a static API key passed in the Api-Key header.\n  Keys are generated in the Bridge dashboard and may be unrestricted or scoped to a\n \
  \ subset of the 68 available scopes. Sandbox keys are prefixed sk-test and target\n  the sandbox base URL. There is no OAuth2 / OpenID Connect flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge/refs/heads/main/authentication/bridge-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Crypto
- Stablecoins
- Payments
- Money Movement
- Cross-Border Payments
- Virtual Accounts
- Wallets
- Cards
- Fintech
---
