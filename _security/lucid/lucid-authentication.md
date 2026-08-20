---
api_key_in: []
api_specs:
- filename: lucid-rest-api-openapi.yml
  format: yaml
  label: Lucid REST API
  slug: lucid-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-rest-api-openapi.yml
- filename: lucid-data-api-openapi.yml
  format: yaml
  label: Lucid Data API
  slug: lucid-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-data-api-openapi.yml
- filename: lucid-scim-api-openapi.yml
  format: yaml
  label: Lucid SCIM API
  slug: lucid-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-scim-api-openapi.yml
- filename: lucid-chatgpt-plugin-openapi.yaml
  format: yaml
  label: Lucid ChatGPT Plugin API
  slug: lucid-chatgpt-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/openapi/lucid-chatgpt-plugin-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lucid Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Lucid secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Lucid
provider_slug: lucid
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://lucid.app/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.lucid.co/oauth2/token
  name: OAuth2
  sources:
  - openapi/lucid-data-api-openapi.yml
  - openapi/lucid-rest-api-openapi.yml
  type: oauth2
- name: ApiKey
  scheme: bearer
  sources:
  - openapi/lucid-rest-api-openapi.yml
  - openapi/lucid-scim-api-openapi.yml
  type: http
slug: lucid-authentication
source_filename: lucid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/lucid-data-api-openapi.yml, openapi/lucid-rest-api-openapi.yml, openapi/lucid-scim-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://lucid.app/oauth2/authorize\n    tokenUrl: https://api.lucid.co/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/lucid-data-api-openapi.yml\n  - openapi/lucid-rest-api-openapi.yml\n- name: ApiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/lucid-rest-api-openapi.yml\n  - openapi/lucid-scim-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucid/refs/heads/main/authentication/lucid-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Visual Collaboration
- Diagramming
- Whiteboarding
- Productivity
- Software-as-a-Service
- Cloud Visualization
- SCIM
- Identity
- Data
- MCP
---
