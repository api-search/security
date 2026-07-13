---
api_key_in:
- header
api_specs:
- filename: ironclad-public-api-openapi.yml
  format: yaml
  label: Ironclad Public API
  slug: ironclad-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-public-api-openapi.yml
- filename: ironclad-oauth-20-api-openapi.yml
  format: yaml
  label: Ironclad OAuth 2.0 API
  slug: ironclad-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-oauth-20-api-openapi.yml
- filename: ironclad-scim-api-openapi.yml
  format: yaml
  label: Ironclad SCIM 2.0 API
  slug: ironclad-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/openapi/ironclad-scim-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ironclad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Ironclad secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Ironclad
provider_slug: ironclad
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: Authorization
  sources:
  - openapi/ironclad-public-api-openapi.yml
  - openapi/ironclad-scim-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://na1.ironcladapp.com/oauth/authorize
    flow: authorizationCode
    scopes: 60
    tokenUrl: https://na1.ironcladapp.com/oauth/token
  - flow: clientCredentials
    scopes: 58
    tokenUrl: https://na1.ironcladapp.com/oauth/token
  name: OAuth2
  sources:
  - openapi/ironclad-public-api-openapi.yml
  type: oauth2
slug: ironclad-authentication
source_filename: ironclad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ironclad-public-api-openapi.yml, openapi/ironclad-scim-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n  - openapi/ironclad-scim-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://na1.ironcladapp.com/oauth/authorize\n    tokenUrl: https://na1.ironcladapp.com/oauth/token\n    scopes: 60\n  - flow: clientCredentials\n    tokenUrl: https://na1.ironcladapp.com/oauth/token\n    scopes: 58\n  sources:\n  - openapi/ironclad-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironclad/refs/heads/main/authentication/ironclad-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Contract Lifecycle Management
- CLM
- Contracts
- Legal Tech
- LegalOps
- Enterprise
- Workflows
- eSignature
- Clickwrap
- AI
- OAuth
- SCIM
- Webhooks
---
