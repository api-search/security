---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: beancount-io-ledger-api-openapi.yml
  format: yaml
  label: Beancount.io Ledger API
  slug: beancount-io-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-ledger-api-openapi.yml
- filename: beancount-io-mcp-api-openapi.yml
  format: yaml
  label: Beancount.io MCP API
  slug: beancount-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-mcp-api-openapi.yml
- filename: beancount-io-graph-ql-api-openapi.yml
  format: yaml
  label: Beancount.io Graph QL API
  slug: beancount-io-graph-ql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beancount-io/openapi/beancount-io-graph-ql-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Beancount.io Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Beancount.io secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Beancount.io
provider_slug: beancount-io
scheme_count: 2
schemes:
- description: 'Scoped API key. Roles: read (query content/ledgers), write (ledger edits), admin (full). Request only needed scopes. Self-serve keys via dashboard; free tier and sandbox available at /demo. Rotate via API.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/beancount-io-openapi.json
  type: apiKey
- description: OAuth 2.1 with PKCE for MCP and GraphQL. Scopes enforce least privilege.
  flows:
  - authorizationUrl: https://beancount.io/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://beancount.io/oauth/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://beancount.io/oauth/token
  name: OAuth2
  sources:
  - openapi/beancount-io-openapi.json
  type: oauth2
slug: beancount-io-authentication
source_filename: beancount-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/beancount-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Scoped API key. Roles: read (query content/ledgers), write (ledger edits), admin\n    (full). Request only needed scopes. Self-serve keys via dashboard; free tier and sandbox\n    available at /demo. Rotate via API.'\n  sources:\n  - openapi/beancount-io-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://beancount.io/oauth/authorize\n    tokenUrl: https://beancount.io/oauth/token\n    scopes: 3\n  - flow: clientCredentials\n    tokenUrl: https://beancount.io/oauth/token\n    scopes: 2\n  description: OAuth 2.1 with PKCE for MCP and GraphQL. Scopes enforce least privilege.\n  sources:\n  - openapi/beancount-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/beancount-io/authentication/beancount-io-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Accounting
- Finance
- Software-as-a-Service
- Open Source
- Collaboration
---
