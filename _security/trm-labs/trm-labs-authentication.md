---
api_key_in: []
api_specs:
- filename: trm-labs-sanctions-openapi.yml
  format: yaml
  label: TRM Sanctions API
  slug: trm-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trm-labs/refs/heads/main/openapi/trm-labs-sanctions-openapi.yml
- filename: trm-labs-chainabuse-openapi.yml
  format: yaml
  label: Chainabuse Public API
  slug: chainabuse-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trm-labs/refs/heads/main/openapi/trm-labs-chainabuse-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Trm Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: TRM Labs secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TRM Labs
provider_slug: trm-labs
scheme_count: 2
schemes:
- api: TRM Sanctions API
  description: TRM Sanctions API uses HTTP Basic authentication with the API key supplied as both username and password. Request an API key at https://www.trmlabs.com/products/sanctions.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/trm-labs-sanctions-openapi.yml
  type: http
- api: Chainabuse Public API
  description: Chainabuse Public API uses HTTP Basic authentication. Credentials are generated from your Chainabuse user profile and passed in the Authorization header as base64-encoded credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/trm-labs-chainabuse-openapi.yml
  type: http
slug: trm-labs-authentication
source_filename: trm-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.trmlabs.com/guides/chainabuse/getting-started\ndocs: https://docs.trmlabs.com/guides/chainabuse/getting-started\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      TRM Sanctions API uses HTTP Basic authentication with the API key supplied\n      as both username and password. Request an API key at\n      https://www.trmlabs.com/products/sanctions.\n    sources: [openapi/trm-labs-sanctions-openapi.yml]\n    api: TRM Sanctions API\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      Chainabuse Public API uses HTTP Basic authentication. Credentials are\n      generated from your Chainabuse user profile and passed in the\n      Authorization header as base64-encoded credentials.\n    sources: [openapi/trm-labs-chainabuse-openapi.yml]\n    api: Chainabuse\
  \ Public API\nnotes: >-\n  Both public TRM Labs APIs authenticate with HTTP Basic. There is no documented\n  OAuth2/OIDC surface, so no scopes artifact applies.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trm-labs/refs/heads/main/authentication/trm-labs-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Crypto
- Blockchain
- Compliance
- Sanctions
- Fraud
- Anti-Money Laundering
- Blockchain Intelligence
---
