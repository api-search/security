---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cuvo-co-a2a-api-openapi.yml
  format: yaml
  label: Cuvo Health A2a API
  slug: cuvo-co-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-a2a-api-openapi.yml
- filename: cuvo-co-acp-api-openapi.yml
  format: yaml
  label: Cuvo Health Acp API
  slug: cuvo-co-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-acp-api-openapi.yml
- filename: cuvo-co-content-api-openapi.yml
  format: yaml
  label: Cuvo Health Content API
  slug: cuvo-co-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-content-api-openapi.yml
- filename: cuvo-co-discovery-api-openapi.yml
  format: yaml
  label: Cuvo Health Discovery API
  slug: cuvo-co-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-discovery-api-openapi.yml
- filename: cuvo-co-mcp-api-openapi.yml
  format: yaml
  label: Cuvo Health MCP API
  slug: cuvo-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-mcp-api-openapi.yml
- filename: cuvo-co-status-api-openapi.yml
  format: yaml
  label: Cuvo Health Status API
  slug: cuvo-co-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-status-api-openapi.yml
auth_types: []
description: 'Cuvo Health supports two authentication mechanisms: API keys and OAuth 2.0 clients.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cuvo Co Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cuvo Health declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cuvo Health
provider_slug: cuvo-co
scheme_count: 2
schemes:
- evidence: 'Every request to https://api.cuvo.co carries Authorization: Bearer <credential> .'
  header: Authorization
  how_to_obtain: Mint an API key in the developer portal behind a multi‑factor challenge; the plaintext key is shown once and prefixed with cuvo_sk_test_ for sandbox or cuvo_sk_live_ for production.
  location: header
  name: API Key
  type: http-bearer
- evidence: 'Exchange the client credentials for an access token:'
  flows:
  - client_credentials
  - device_code
  header: Authorization
  how_to_obtain: Create an OAuth client at /portal/<integration>/oauth-clients; you receive a client_id and a client_secret shown once.
  location: header
  name: OAuth client
  scopes:
  - patients:write
  - cases:write
  - events:read
  token_url: https://developers.cuvo.co/api/auth/oauth2/token
  type: oauth2
slug: cuvo-co-authentication
source_filename: cuvo-co-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.cuvo.co/docs/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.cuvo.co/docs/authentication\nsources:\n- https://developers.cuvo.co/docs/authentication\n- https://developers.cuvo.co/docs/getting-started\ndescription: 'Cuvo Health supports two authentication mechanisms: API keys and OAuth 2.0 clients.'\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Every request to https://api.cuvo.co carries Authorization: Bearer <credential> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint an API key in the developer portal behind a multi‑factor challenge; the plaintext key is shown once and prefixed with cuvo_sk_test_\n    for sandbox or cuvo_sk_live_ for production.\n- type: oauth2\n  name: OAuth client\n  evidence: 'Exchange the client credentials for an access token:'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  - device_code\n  token_url: https://developers.cuvo.co/api/auth/oauth2/token\n\
  \  scopes:\n  - patients:write\n  - cases:write\n  - events:read\n  how_to_obtain: Create an OAuth client at /portal/<integration>/oauth-clients; you receive a client_id and a client_secret shown once.\ndocs: https://developers.cuvo.co/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/cuvo-co/authentication/cuvo-co-authentication.yml
summary_line: 2 schemes
tags:
- Telehealth
- White‑Label Platform
- Pharmacy Fulfillment
- Brand Licensing
---
