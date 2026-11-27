---
anonymous_access: false
api_key_in: []
api_specs:
- filename: convexlake-com-openapi-generated.yml
  format: yaml
  label: Convex Lake API
  slug: convexlake-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convexlake-com/openapi/_ae-authored/convexlake-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Convex Lake Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convex Lake declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Convex Lake
provider_slug: convexlake-com
scheme_count: 1
schemes:
- description: 'Generate an API key on the API Keys page (Settings → API Keys). Keys look like do_XXXXXXXX_XXXXXXXX and are shown only once. Every request carries the key in a header: x-api-key. Use x-api-key, not Authorization.'
  in: header
  key_format: do_XXXXXXXX_XXXXXXXX
  name: apiKey
  parameter: x-api-key
  revocation: Keys can be revoked at any time from the API Keys page. Revoked keys are immediately rejected.
  rotation: 'Rotate keys periodically: generate a new key first, migrate your clients, then revoke the old one.'
  tiering: The key's subscription tier decides which exchanges it can read (/info returns tier and allowed_exchanges).
  type: apiKey
slug: convexlake-com-authentication
source_filename: convexlake-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://convexlake.com/docs\ndocs: https://convexlake.com/docs\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Generate an API key on the API Keys page (Settings → API Keys). Keys look like do_XXXXXXXX_XXXXXXXX and are shown only once. Every request carries the key in a header: x-api-key. Use x-api-key, not Authorization.'\n  key_format: do_XXXXXXXX_XXXXXXXX\n  revocation: Keys can be revoked at any time from the API Keys page. Revoked keys are immediately rejected.\n  rotation: 'Rotate keys periodically: generate a new key first, migrate your clients, then revoke the old one.'\n  tiering: The key's subscription tier decides which exchanges it can read (/info returns tier and allowed_exchanges).\noauth: false\n"
source_yaml_url: https://artifacts.apis.io/convexlake-com/authentication/convexlake-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Market Data
- Prediction Markets
- Orderbook Data
- Quantitative Finance
- Cryptocurrency
- Derivatives
- Historical Data
- MCP
---
